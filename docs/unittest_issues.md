# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [csharp/compatibility_tests/v3.0.0/protos/csharp/protos/unittest_issues.proto](#csharp_compatibility_tests_v3-0-0_protos_csharp_protos_unittest_issues-proto)
    - [DeprecatedChild](#unittest_issues-DeprecatedChild)
    - [DeprecatedFieldsMessage](#unittest_issues-DeprecatedFieldsMessage)
    - [Issue307](#unittest_issues-Issue307)
    - [Issue307.NestedOnce](#unittest_issues-Issue307-NestedOnce)
    - [Issue307.NestedOnce.NestedTwice](#unittest_issues-Issue307-NestedOnce-NestedTwice)
    - [ItemField](#unittest_issues-ItemField)
    - [NegativeEnumMessage](#unittest_issues-NegativeEnumMessage)
    - [ReservedNames](#unittest_issues-ReservedNames)
    - [ReservedNames.SomeNestedType](#unittest_issues-ReservedNames-SomeNestedType)
    - [TestJsonFieldOrdering](#unittest_issues-TestJsonFieldOrdering)
    - [TestJsonName](#unittest_issues-TestJsonName)
  
    - [DeprecatedEnum](#unittest_issues-DeprecatedEnum)
    - [NegativeEnum](#unittest_issues-NegativeEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="csharp_compatibility_tests_v3-0-0_protos_csharp_protos_unittest_issues-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## csharp/compatibility_tests/v3.0.0/protos/csharp/protos/unittest_issues.proto



<a name="unittest_issues-DeprecatedChild"></a>

### DeprecatedChild







<a name="unittest_issues-DeprecatedFieldsMessage"></a>

### DeprecatedFieldsMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| PrimitiveValue | [int32](#int32) |  | **Deprecated.**  |
| PrimitiveArray | [int32](#int32) | repeated | **Deprecated.**  |
| MessageValue | [DeprecatedChild](#unittest_issues-DeprecatedChild) |  | **Deprecated.**  |
| MessageArray | [DeprecatedChild](#unittest_issues-DeprecatedChild) | repeated | **Deprecated.**  |
| EnumValue | [DeprecatedEnum](#unittest_issues-DeprecatedEnum) |  | **Deprecated.**  |
| EnumArray | [DeprecatedEnum](#unittest_issues-DeprecatedEnum) | repeated | **Deprecated.**  |






<a name="unittest_issues-Issue307"></a>

### Issue307
Issue 307: when generating doubly-nested types, any references
should be of the form A.Types.B.Types.C.






<a name="unittest_issues-Issue307-NestedOnce"></a>

### Issue307.NestedOnce







<a name="unittest_issues-Issue307-NestedOnce-NestedTwice"></a>

### Issue307.NestedOnce.NestedTwice







<a name="unittest_issues-ItemField"></a>

### ItemField
Issue 45: http://code.google.com/p/protobuf-csharp-port/issues/detail?id=45


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item | [int32](#int32) |  |  |






<a name="unittest_issues-NegativeEnumMessage"></a>

### NegativeEnumMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [NegativeEnum](#unittest_issues-NegativeEnum) |  |  |
| values | [NegativeEnum](#unittest_issues-NegativeEnum) | repeated |  |
| packed_values | [NegativeEnum](#unittest_issues-NegativeEnum) | repeated |  |






<a name="unittest_issues-ReservedNames"></a>

### ReservedNames



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| types | [int32](#int32) |  |  |
| descriptor | [int32](#int32) |  |  |






<a name="unittest_issues-ReservedNames-SomeNestedType"></a>

### ReservedNames.SomeNestedType
Force a nested type called Types






<a name="unittest_issues-TestJsonFieldOrdering"></a>

### TestJsonFieldOrdering
These fields are deliberately not declared in numeric
order, and the oneof fields aren&#39;t contiguous either.
This allows for reasonably robust tests of JSON output
ordering.
TestFieldOrderings in unittest_proto3.proto is similar,
but doesn&#39;t include oneofs.
TODO: Consider adding oneofs to TestFieldOrderings, although
that will require fixing other tests in multiple platforms.
Alternatively, consider just adding this to
unittest_proto3.proto if multiple platforms want it.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| plain_int32 | [int32](#int32) |  |  |
| o1_string | [string](#string) |  |  |
| o1_int32 | [int32](#int32) |  |  |
| plain_string | [string](#string) |  |  |
| o2_int32 | [int32](#int32) |  |  |
| o2_string | [string](#string) |  |  |






<a name="unittest_issues-TestJsonName"></a>

### TestJsonName



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  | Message for testing the effects for of the json_name option |
| description | [string](#string) |  |  |
| guid | [string](#string) |  |  |





 


<a name="unittest_issues-DeprecatedEnum"></a>

### DeprecatedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| DEPRECATED_ZERO | 0 |  |
| one | 1 |  |



<a name="unittest_issues-NegativeEnum"></a>

### NegativeEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| NEGATIVE_ENUM_ZERO | 0 |  |
| FiveBelow | -5 |  |
| MinusOne | -1 |  |


 

 

 



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

