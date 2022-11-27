# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [ruby/tests/generated_code_proto2.proto](#ruby_tests_generated_code_proto2-proto)
    - [TestMessage](#a-b-proto2-TestMessage)
    - [TestMessage.NestedMessage](#a-b-proto2-TestMessage-NestedMessage)
    - [TestUnknown](#a-b-proto2-TestUnknown)
  
    - [TestEnum](#a-b-proto2-TestEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="ruby_tests_generated_code_proto2-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## ruby/tests/generated_code_proto2.proto



<a name="a-b-proto2-TestMessage"></a>

### TestMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) | optional |  |
| optional_int64 | [int64](#int64) | optional |  |
| optional_uint32 | [uint32](#uint32) | optional |  |
| optional_uint64 | [uint64](#uint64) | optional |  |
| optional_bool | [bool](#bool) | optional |  |
| optional_double | [double](#double) | optional |  |
| optional_float | [float](#float) | optional |  |
| optional_string | [string](#string) | optional |  |
| optional_bytes | [bytes](#bytes) | optional |  |
| optional_enum | [TestEnum](#a-b-proto2-TestEnum) | optional |  |
| optional_msg | [TestMessage](#a-b-proto2-TestMessage) | optional |  |
| repeated_int32 | [int32](#int32) | repeated |  |
| repeated_int64 | [int64](#int64) | repeated |  |
| repeated_uint32 | [uint32](#uint32) | repeated |  |
| repeated_uint64 | [uint64](#uint64) | repeated |  |
| repeated_bool | [bool](#bool) | repeated |  |
| repeated_double | [double](#double) | repeated |  |
| repeated_float | [float](#float) | repeated |  |
| repeated_string | [string](#string) | repeated |  |
| repeated_bytes | [bytes](#bytes) | repeated |  |
| repeated_enum | [TestEnum](#a-b-proto2-TestEnum) | repeated |  |
| repeated_msg | [TestMessage](#a-b-proto2-TestMessage) | repeated |  |
| required_int32 | [int32](#int32) | required |  |
| required_int64 | [int64](#int64) | required |  |
| required_uint32 | [uint32](#uint32) | required |  |
| required_uint64 | [uint64](#uint64) | required |  |
| required_bool | [bool](#bool) | required |  |
| required_double | [double](#double) | required |  |
| required_float | [float](#float) | required |  |
| required_string | [string](#string) | required |  |
| required_bytes | [bytes](#bytes) | required |  |
| required_enum | [TestEnum](#a-b-proto2-TestEnum) | required |  |
| required_msg | [TestMessage](#a-b-proto2-TestMessage) | required |  |
| oneof_int32 | [int32](#int32) | optional |  |
| oneof_int64 | [int64](#int64) | optional |  |
| oneof_uint32 | [uint32](#uint32) | optional |  |
| oneof_uint64 | [uint64](#uint64) | optional |  |
| oneof_bool | [bool](#bool) | optional |  |
| oneof_double | [double](#double) | optional |  |
| oneof_float | [float](#float) | optional |  |
| oneof_string | [string](#string) | optional |  |
| oneof_bytes | [bytes](#bytes) | optional |  |
| oneof_enum | [TestEnum](#a-b-proto2-TestEnum) | optional |  |
| oneof_msg | [TestMessage](#a-b-proto2-TestMessage) | optional |  |
| nested_message | [TestMessage.NestedMessage](#a-b-proto2-TestMessage-NestedMessage) | optional |  |






<a name="a-b-proto2-TestMessage-NestedMessage"></a>

### TestMessage.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [int32](#int32) | optional |  |






<a name="a-b-proto2-TestUnknown"></a>

### TestUnknown



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_unknown | [TestUnknown](#a-b-proto2-TestUnknown) | optional |  |
| repeated_unknown | [TestUnknown](#a-b-proto2-TestUnknown) | repeated |  |
| oneof_unknown | [TestUnknown](#a-b-proto2-TestUnknown) | optional |  |
| unknown_field | [int32](#int32) | optional |  |





 


<a name="a-b-proto2-TestEnum"></a>

### TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| Default | 0 |  |
| A | 1 |  |
| B | 2 |  |
| C | 3 |  |
| v0 | 4 |  |


 

 

 



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

