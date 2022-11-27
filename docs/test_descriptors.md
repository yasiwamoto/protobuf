# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [php/tests/proto/test_descriptors.proto](#php_tests_proto_test_descriptors-proto)
    - [TestDescriptorsMessage](#descriptors-TestDescriptorsMessage)
    - [TestDescriptorsMessage.MapInt32EnumEntry](#descriptors-TestDescriptorsMessage-MapInt32EnumEntry)
    - [TestDescriptorsMessage.Sub](#descriptors-TestDescriptorsMessage-Sub)
  
    - [TestDescriptorsEnum](#descriptors-TestDescriptorsEnum)
    - [TestDescriptorsMessage.EnumSub](#descriptors-TestDescriptorsMessage-EnumSub)
  
- [Scalar Value Types](#scalar-value-types)



<a name="php_tests_proto_test_descriptors-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## php/tests/proto/test_descriptors.proto



<a name="descriptors-TestDescriptorsMessage"></a>

### TestDescriptorsMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) |  |  |
| optional_enum | [TestDescriptorsEnum](#descriptors-TestDescriptorsEnum) |  |  |
| optional_message | [TestDescriptorsMessage.Sub](#descriptors-TestDescriptorsMessage-Sub) |  |  |
| repeated_int32 | [int32](#int32) | repeated | Repeated |
| repeated_message | [TestDescriptorsMessage.Sub](#descriptors-TestDescriptorsMessage-Sub) | repeated |  |
| oneof_int32 | [int32](#int32) |  |  |
| proto3_optional_int32 | [int32](#int32) | optional |  |
| map_int32_enum | [TestDescriptorsMessage.MapInt32EnumEntry](#descriptors-TestDescriptorsMessage-MapInt32EnumEntry) | repeated |  |






<a name="descriptors-TestDescriptorsMessage-MapInt32EnumEntry"></a>

### TestDescriptorsMessage.MapInt32EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestDescriptorsMessage.EnumSub](#descriptors-TestDescriptorsMessage-EnumSub) |  |  |






<a name="descriptors-TestDescriptorsMessage-Sub"></a>

### TestDescriptorsMessage.Sub



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) |  |  |
| b | [int32](#int32) | repeated |  |





 


<a name="descriptors-TestDescriptorsEnum"></a>

### TestDescriptorsEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |



<a name="descriptors-TestDescriptorsMessage-EnumSub"></a>

### TestDescriptorsMessage.EnumSub


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |


 

 

 



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

