# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [conformance/conformance.proto](#conformance_conformance-proto)
    - [ConformanceRequest](#conformance-ConformanceRequest)
    - [ConformanceResponse](#conformance-ConformanceResponse)
    - [FailureSet](#conformance-FailureSet)
    - [JspbEncodingConfig](#conformance-JspbEncodingConfig)
  
    - [TestCategory](#conformance-TestCategory)
    - [WireFormat](#conformance-WireFormat)
  
- [Scalar Value Types](#scalar-value-types)



<a name="conformance_conformance-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## conformance/conformance.proto



<a name="conformance-ConformanceRequest"></a>

### ConformanceRequest
Represents a single test case&#39;s input.  The testee should:

  1. parse this proto (which should always succeed)
  2. parse the protobuf or JSON payload in &#34;payload&#34; (which may fail)
  3. if the parse succeeded, serialize the message in the requested format.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| protobuf_payload | [bytes](#bytes) |  |  |
| json_payload | [string](#string) |  |  |
| jspb_payload | [string](#string) |  | Only used inside Google. Opensource testees just skip it. |
| text_payload | [string](#string) |  |  |
| requested_output_format | [WireFormat](#conformance-WireFormat) |  | Which format should the testee serialize its message to? |
| message_type | [string](#string) |  | The full name for the test message to use; for the moment, either: protobuf_test_messages.proto3.TestAllTypesProto3 or protobuf_test_messages.google.protobuf.TestAllTypesProto2. |
| test_category | [TestCategory](#conformance-TestCategory) |  | Each test is given a specific test category. Some category may need specific support in testee programs. Refer to the definition of TestCategory for more information. |
| jspb_encoding_options | [JspbEncodingConfig](#conformance-JspbEncodingConfig) |  | Specify details for how to encode jspb. |
| print_unknown_fields | [bool](#bool) |  | This can be used in json and text format. If true, testee should print unknown fields instead of ignore. This feature is optional. |






<a name="conformance-ConformanceResponse"></a>

### ConformanceResponse
Represents a single test case&#39;s output.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| parse_error | [string](#string) |  | This string should be set to indicate parsing failed. The string can provide more information about the parse error if it is available.

Setting this string does not necessarily mean the testee failed the test. Some of the test cases are intentionally invalid input. |
| serialize_error | [string](#string) |  | If the input was successfully parsed but errors occurred when serializing it to the requested output format, set the error message in this field. |
| timeout_error | [string](#string) |  | This should be set if the test program timed out. The string should provide more information about what the child process was doing when it was killed. |
| runtime_error | [string](#string) |  | This should be set if some other error occurred. This will always indicate that the test failed. The string can provide more information about the failure. |
| protobuf_payload | [bytes](#bytes) |  | If the input was successfully parsed and the requested output was protobuf, serialize it to protobuf and set it in this field. |
| json_payload | [string](#string) |  | If the input was successfully parsed and the requested output was JSON, serialize to JSON and set it in this field. |
| skipped | [string](#string) |  | For when the testee skipped the test, likely because a certain feature wasn&#39;t supported, like JSON input/output. |
| jspb_payload | [string](#string) |  | If the input was successfully parsed and the requested output was JSPB, serialize to JSPB and set it in this field. JSPB is only used inside Google. Opensource testees can just skip it. |
| text_payload | [string](#string) |  | If the input was successfully parsed and the requested output was TEXT_FORMAT, serialize to TEXT_FORMAT and set it in this field. |






<a name="conformance-FailureSet"></a>

### FailureSet
The conformance runner will request a list of failures as the first request.
This will be known by message_type == &#34;conformance.FailureSet&#34;, a conformance
test should return a serialized FailureSet in protobuf_payload.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| failure | [string](#string) | repeated |  |






<a name="conformance-JspbEncodingConfig"></a>

### JspbEncodingConfig
Encoding options for jspb format.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| use_jspb_array_any_format | [bool](#bool) |  | Encode the value field of Any as jspb array if true, otherwise binary. |





 


<a name="conformance-TestCategory"></a>

### TestCategory


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNSPECIFIED_TEST | 0 |  |
| BINARY_TEST | 1 | Test binary wire format. |
| JSON_TEST | 2 | Test json wire format. |
| JSON_IGNORE_UNKNOWN_PARSING_TEST | 3 | Similar to JSON_TEST. However, during parsing json, testee should ignore unknown fields. This feature is optional. Each implementation can decide whether to support it. See https://developers.google.com/protocol-buffers/docs/proto3#json_options for more detail. |
| JSPB_TEST | 4 | Test jspb wire format. Only used inside Google. Opensource testees just skip it. |
| TEXT_FORMAT_TEST | 5 | Test text format. For cpp, java and python, testees can already deal with this type. Testees of other languages can simply skip it. |



<a name="conformance-WireFormat"></a>

### WireFormat


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNSPECIFIED | 0 |  |
| PROTOBUF | 1 |  |
| JSON | 2 |  |
| JSPB | 3 | Only used inside Google. Opensource testees just skip it. |
| TEXT_FORMAT | 4 |  |


 

 

 



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

