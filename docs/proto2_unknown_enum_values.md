# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/core/src/test/proto/com/google/protobuf/proto2_unknown_enum_values.proto](#java_core_src_test_proto_com_google_protobuf_proto2_unknown_enum_values-proto)
    - [Proto2EnumMessage](#proto2_unknown_enum_values-Proto2EnumMessage)
    - [Proto2EnumMessageWithEnumSubset](#proto2_unknown_enum_values-Proto2EnumMessageWithEnumSubset)
  
    - [Proto2TestEnum](#proto2_unknown_enum_values-Proto2TestEnum)
    - [Proto2TestEnumSubset](#proto2_unknown_enum_values-Proto2TestEnumSubset)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_core_src_test_proto_com_google_protobuf_proto2_unknown_enum_values-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/core/src/test/proto/com/google/protobuf/proto2_unknown_enum_values.proto



<a name="proto2_unknown_enum_values-Proto2EnumMessage"></a>

### Proto2EnumMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| repeated_packed_enum | [Proto2TestEnum](#proto2_unknown_enum_values-Proto2TestEnum) | repeated |  |






<a name="proto2_unknown_enum_values-Proto2EnumMessageWithEnumSubset"></a>

### Proto2EnumMessageWithEnumSubset
Test messages for packed enum, with identical field number as
Proto2Message, to test parsing unknown packed enums.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| repeated_packed_enum | [Proto2TestEnumSubset](#proto2_unknown_enum_values-Proto2TestEnumSubset) | repeated |  |





 


<a name="proto2_unknown_enum_values-Proto2TestEnum"></a>

### Proto2TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |
| TWO | 2 |  |



<a name="proto2_unknown_enum_values-Proto2TestEnumSubset"></a>

### Proto2TestEnumSubset
An enum containing a subset of the values of Proto2TestEnum, to test
parsing unknown packed enum values

| Name | Number | Description |
| ---- | ------ | ----------- |
| TESTENUM_SUBSET_ZERO | 0 |  |
| TESTENUM_SUBSET_ONE | 1 | No enum value with number 2. |


 

 

 



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

