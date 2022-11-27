# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_deprecated.proto](#objectivec_Tests_unittest_deprecated-proto)
    - [Msg1](#objc-protobuf-tests-deprecated-Msg1)
    - [Msg1A](#objc-protobuf-tests-deprecated-Msg1A)
    - [Msg2](#objc-protobuf-tests-deprecated-Msg2)
  
    - [Enum1](#objc-protobuf-tests-deprecated-Enum1)
    - [Enum2](#objc-protobuf-tests-deprecated-Enum2)
  
    - [File-level Extensions](#objectivec_Tests_unittest_deprecated-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_deprecated-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_deprecated-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_deprecated-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_deprecated-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_deprecated.proto



<a name="objc-protobuf-tests-deprecated-Msg1"></a>

### Msg1
Mix of field types marked as deprecated.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| string_field | [string](#string) | optional | **Deprecated.**  |
| int_field | [int32](#int32) | required | **Deprecated.**  |
| fixed_field | [fixed32](#fixed32) | repeated | **Deprecated.**  |
| msg_field | [Msg1](#objc-protobuf-tests-deprecated-Msg1) | optional | **Deprecated.**  |






<a name="objc-protobuf-tests-deprecated-Msg1A"></a>

### Msg1A
Mix of extension field types (scoped to a message) marked as deprecated.




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| string_ext2_field | string | Msg1 | 201 |  |
| int_ext2_field | int32 | Msg1 | 202 |  |
| fixed_ext2_field | fixed32 | Msg1 | 203 |  |
| msg_ext2_field | Msg1 | Msg1 | 204 |  |




<a name="objc-protobuf-tests-deprecated-Msg2"></a>

### Msg2
Message marked as deprecated.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| string_field | [string](#string) | optional |  |
| int_field | [int32](#int32) | required |  |
| fixed_field | [fixed32](#fixed32) | repeated |  |





 


<a name="objc-protobuf-tests-deprecated-Enum1"></a>

### Enum1
Enum value marked as deprecated.

| Name | Number | Description |
| ---- | ------ | ----------- |
| ENUM1_ONE | 1 |  |
| ENUM1_TWO | 2 |  |
| ENUM1_THREE | 3 |  |



<a name="objc-protobuf-tests-deprecated-Enum2"></a>

### Enum2
Enum marked as deprecated.

| Name | Number | Description |
| ---- | ------ | ----------- |
| ENUM2_ONE | 1 |  |
| ENUM2_TWO | 2 |  |
| ENUM2_THREE | 3 |  |


 


<a name="objectivec_Tests_unittest_deprecated-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| fixed_ext_field | fixed32 | Msg1 | 103 |  |
| int_ext_field | int32 | Msg1 | 102 |  |
| msg_ext_field | Msg1 | Msg1 | 104 |  |
| string_ext_field | string | Msg1 | 101 |  |

 

 



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

