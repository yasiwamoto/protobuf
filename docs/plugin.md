# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [src/google/protobuf/compiler/plugin.proto](#src_google_protobuf_compiler_plugin-proto)
    - [CodeGeneratorRequest](#google-protobuf-compiler-CodeGeneratorRequest)
    - [CodeGeneratorResponse](#google-protobuf-compiler-CodeGeneratorResponse)
    - [CodeGeneratorResponse.File](#google-protobuf-compiler-CodeGeneratorResponse-File)
    - [Version](#google-protobuf-compiler-Version)
  
    - [CodeGeneratorResponse.Feature](#google-protobuf-compiler-CodeGeneratorResponse-Feature)
  
- [Scalar Value Types](#scalar-value-types)



<a name="src_google_protobuf_compiler_plugin-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## src/google/protobuf/compiler/plugin.proto



<a name="google-protobuf-compiler-CodeGeneratorRequest"></a>

### CodeGeneratorRequest
An encoded CodeGeneratorRequest is written to the plugin&#39;s stdin.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| file_to_generate | [string](#string) | repeated | The .proto files that were explicitly listed on the command-line. The code generator should generate code only for these files. Each file&#39;s descriptor will be included in proto_file, below. |
| parameter | [string](#string) | optional | The generator parameter passed on the command-line. |
| proto_file | [google.protobuf.FileDescriptorProto](#google-protobuf-FileDescriptorProto) | repeated | FileDescriptorProtos for all files in files_to_generate and everything they import. The files will appear in topological order, so each file appears before any file that imports it.

protoc guarantees that all proto_files will be written after the fields above, even though this is not technically guaranteed by the protobuf wire format. This theoretically could allow a plugin to stream in the FileDescriptorProtos and handle them one by one rather than read the entire set into memory at once. However, as of this writing, this is not similarly optimized on protoc&#39;s end -- it will store all fields in memory at once before sending them to the plugin.

Type names of fields and extensions in the FileDescriptorProto are always fully qualified. |
| compiler_version | [Version](#google-protobuf-compiler-Version) | optional | The version number of protocol compiler. |






<a name="google-protobuf-compiler-CodeGeneratorResponse"></a>

### CodeGeneratorResponse
The plugin writes an encoded CodeGeneratorResponse to stdout.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| error | [string](#string) | optional | Error message. If non-empty, code generation failed. The plugin process should exit with status code zero even if it reports an error in this way.

This should be used to indicate errors in .proto files which prevent the code generator from generating correct code. Errors which indicate a problem in protoc itself -- such as the input CodeGeneratorRequest being unparseable -- should be reported by writing a message to stderr and exiting with a non-zero status code. |
| supported_features | [uint64](#uint64) | optional | A bitmask of supported features that the code generator supports. This is a bitwise &#34;or&#34; of values from the Feature enum. |
| file | [CodeGeneratorResponse.File](#google-protobuf-compiler-CodeGeneratorResponse-File) | repeated |  |






<a name="google-protobuf-compiler-CodeGeneratorResponse-File"></a>

### CodeGeneratorResponse.File
Represents a single generated file.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) | optional | The file name, relative to the output directory. The name must not contain &#34;.&#34; or &#34;..&#34; components and must be relative, not be absolute (so, the file cannot lie outside the output directory). &#34;/&#34; must be used as the path separator, not &#34;\&#34;.

If the name is omitted, the content will be appended to the previous file. This allows the generator to break large files into small chunks, and allows the generated text to be streamed back to protoc so that large files need not reside completely in memory at one time. Note that as of this writing protoc does not optimize for this -- it will read the entire CodeGeneratorResponse before writing files to disk. |
| insertion_point | [string](#string) | optional | If non-empty, indicates that the named file should already exist, and the content here is to be inserted into that file at a defined insertion point. This feature allows a code generator to extend the output produced by another code generator. The original generator may provide insertion points by placing special annotations in the file that look like: @@protoc_insertion_point(NAME) The annotation can have arbitrary text before and after it on the line, which allows it to be placed in a comment. NAME should be replaced with an identifier naming the point -- this is what other generators will use as the insertion_point. Code inserted at this point will be placed immediately above the line containing the insertion point (thus multiple insertions to the same point will come out in the order they were added). The double-@ is intended to make it unlikely that the generated code could contain things that look like insertion points by accident.

For example, the C&#43;&#43; code generator places the following line in the .pb.h files that it generates: // @@protoc_insertion_point(namespace_scope) This line appears within the scope of the file&#39;s package namespace, but outside of any particular class. Another plugin can then specify the insertion_point &#34;namespace_scope&#34; to generate additional classes or other declarations that should be placed in this scope.

Note that if the line containing the insertion point begins with whitespace, the same whitespace will be added to every line of the inserted text. This is useful for languages like Python, where indentation matters. In these languages, the insertion point comment should be indented the same amount as any inserted code will need to be in order to work correctly in that context.

The code generator that generates the initial file and the one which inserts into it must both run as part of a single invocation of protoc. Code generators are executed in the order in which they appear on the command line.

If |insertion_point| is present, |name| must also be present. |
| content | [string](#string) | optional | The file contents. |
| generated_code_info | [google.protobuf.GeneratedCodeInfo](#google-protobuf-GeneratedCodeInfo) | optional | Information describing the file content being inserted. If an insertion point is used, this information will be appropriately offset and inserted into the code generation metadata for the generated files. |






<a name="google-protobuf-compiler-Version"></a>

### Version
The version number of protocol compiler.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| major | [int32](#int32) | optional |  |
| minor | [int32](#int32) | optional |  |
| patch | [int32](#int32) | optional |  |
| suffix | [string](#string) | optional | A suffix for alpha, beta or rc release, e.g., &#34;alpha-1&#34;, &#34;rc2&#34;. It should be empty for mainline stable releases. |





 


<a name="google-protobuf-compiler-CodeGeneratorResponse-Feature"></a>

### CodeGeneratorResponse.Feature
Sync with code_generator.h.

| Name | Number | Description |
| ---- | ------ | ----------- |
| FEATURE_NONE | 0 |  |
| FEATURE_PROTO3_OPTIONAL | 1 |  |


 

 

 



## Scalar Value Types

| .proto Type | Notes | C++ | Java | Python | Go | C# | PHP | Ruby |
| ----------- | ----- | --- | ---- | ------ | -- | -- | --- | ---- |
| <a name="double" /> double |  | double | double | float | float64 | double | float | Float |
| <a name="float" /> float |  | float | float | float | float32 | float | float | Float |
| <a name="int32" /> int32 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="int64" /> int64 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="uint32" /> uint32 | Uses variable-length encoding. | uint32 | int | int/long | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="uint64" /> uint64 | Uses variable-length encoding. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum or Fixnum (as required) |
| <a name="sint32" /> sint32 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sint64" /> sint64 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="fixed32" /> fixed32 | Always four bytes. More efficient than uint32 if values are often greater than 2^28. | uint32 | int | int | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="fixed64" /> fixed64 | Always eight bytes. More efficient than uint64 if values are often greater than 2^56. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum |
| <a name="sfixed32" /> sfixed32 | Always four bytes. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sfixed64" /> sfixed64 | Always eight bytes. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="bool" /> bool |  | bool | boolean | boolean | bool | bool | boolean | TrueClass/FalseClass |
| <a name="string" /> string | A string must always contain UTF-8 encoded or 7-bit ASCII text. | string | String | str/unicode | string | string | string | String (UTF-8) |
| <a name="bytes" /> bytes | May contain any arbitrary sequence of bytes. | string | ByteString | str | []byte | ByteString | string | String (ASCII-8BIT) |

