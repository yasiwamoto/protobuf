# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [python/google/protobuf/pyext/python.proto](#python_google_protobuf_pyext_python-proto)
    - [ForeignMessage](#google-protobuf-python-internal-ForeignMessage)
    - [TestAllExtensions](#google-protobuf-python-internal-TestAllExtensions)
    - [TestAllTypes](#google-protobuf-python-internal-TestAllTypes)
    - [TestAllTypes.NestedMessage](#google-protobuf-python-internal-TestAllTypes-NestedMessage)
  
    - [File-level Extensions](#python_google_protobuf_pyext_python-proto-extensions)
    - [File-level Extensions](#python_google_protobuf_pyext_python-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="python_google_protobuf_pyext_python-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## python/google/protobuf/pyext/python.proto



<a name="google-protobuf-python-internal-ForeignMessage"></a>

### ForeignMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| c | [int32](#int32) | optional |  |
| d | [int32](#int32) | repeated |  |






<a name="google-protobuf-python-internal-TestAllExtensions"></a>

### TestAllExtensions
extension begin






<a name="google-protobuf-python-internal-TestAllTypes"></a>

### TestAllTypes



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| repeated_nested_message | [TestAllTypes.NestedMessage](#google-protobuf-python-internal-TestAllTypes-NestedMessage) | repeated |  |
| optional_nested_message | [TestAllTypes.NestedMessage](#google-protobuf-python-internal-TestAllTypes-NestedMessage) | optional |  |
| optional_int32 | [int32](#int32) | optional |  |






<a name="google-protobuf-python-internal-TestAllTypes-NestedMessage"></a>

### TestAllTypes.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bb | [int32](#int32) | optional |  |
| cc | [ForeignMessage](#google-protobuf-python-internal-ForeignMessage) | optional |  |





 

 


<a name="python_google_protobuf_pyext_python-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| optional_nested_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 1 |  |
| repeated_nested_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 2 |  |

 

 



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

