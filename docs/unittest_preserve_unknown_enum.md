# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_preserve_unknown_enum.proto](#objectivec_Tests_unittest_preserve_unknown_enum-proto)
    - [MyMessage](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyMessage)
    - [MyMessagePlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyMessagePlusExtra)
  
    - [MyEnum](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum)
    - [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_preserve_unknown_enum-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_preserve_unknown_enum.proto



<a name="objc-protobuf-tests-proto3_preserve_unknown_enum-MyMessage"></a>

### MyMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| e | [MyEnum](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum) |  |  |
| repeated_e | [MyEnum](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum) | repeated |  |
| repeated_packed_e | [MyEnum](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum) | repeated |  |
| repeated_packed_unexpected_e | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) | repeated | not packed |
| oneof_e_1 | [MyEnum](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum) |  |  |
| oneof_e_2 | [MyEnum](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum) |  |  |






<a name="objc-protobuf-tests-proto3_preserve_unknown_enum-MyMessagePlusExtra"></a>

### MyMessagePlusExtra



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| e | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) |  |  |
| repeated_e | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) | repeated |  |
| repeated_packed_e | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) | repeated |  |
| repeated_packed_unexpected_e | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) | repeated |  |
| oneof_e_1 | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) |  |  |
| oneof_e_2 | [MyEnumPlusExtra](#objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra) |  |  |





 


<a name="objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnum"></a>

### MyEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |
| BAR | 1 |  |
| BAZ | 2 |  |



<a name="objc-protobuf-tests-proto3_preserve_unknown_enum-MyEnumPlusExtra"></a>

### MyEnumPlusExtra


| Name | Number | Description |
| ---- | ------ | ----------- |
| E_FOO | 0 |  |
| E_BAR | 1 |  |
| E_BAZ | 2 |  |
| E_EXTRA | 3 |  |


 

 

 



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

