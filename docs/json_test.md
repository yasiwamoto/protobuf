# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/util/src/test/proto/com/google/protobuf/util/json_test.proto](#java_util_src_test_proto_com_google_protobuf_util_json_test-proto)
    - [TestAllTypes](#json_test-TestAllTypes)
    - [TestAllTypes.NestedMessage](#json_test-TestAllTypes-NestedMessage)
    - [TestAny](#json_test-TestAny)
    - [TestAny.AnyMapEntry](#json_test-TestAny-AnyMapEntry)
    - [TestCustomJsonName](#json_test-TestCustomJsonName)
    - [TestDuration](#json_test-TestDuration)
    - [TestFieldMask](#json_test-TestFieldMask)
    - [TestMap](#json_test-TestMap)
    - [TestMap.BoolToInt32MapEntry](#json_test-TestMap-BoolToInt32MapEntry)
    - [TestMap.Fixed32ToInt32MapEntry](#json_test-TestMap-Fixed32ToInt32MapEntry)
    - [TestMap.Fixed64ToInt32MapEntry](#json_test-TestMap-Fixed64ToInt32MapEntry)
    - [TestMap.Int32ToBoolMapEntry](#json_test-TestMap-Int32ToBoolMapEntry)
    - [TestMap.Int32ToBytesMapEntry](#json_test-TestMap-Int32ToBytesMapEntry)
    - [TestMap.Int32ToDoubleMapEntry](#json_test-TestMap-Int32ToDoubleMapEntry)
    - [TestMap.Int32ToEnumMapEntry](#json_test-TestMap-Int32ToEnumMapEntry)
    - [TestMap.Int32ToFixed32MapEntry](#json_test-TestMap-Int32ToFixed32MapEntry)
    - [TestMap.Int32ToFixed64MapEntry](#json_test-TestMap-Int32ToFixed64MapEntry)
    - [TestMap.Int32ToFloatMapEntry](#json_test-TestMap-Int32ToFloatMapEntry)
    - [TestMap.Int32ToInt32MapEntry](#json_test-TestMap-Int32ToInt32MapEntry)
    - [TestMap.Int32ToInt64MapEntry](#json_test-TestMap-Int32ToInt64MapEntry)
    - [TestMap.Int32ToMessageMapEntry](#json_test-TestMap-Int32ToMessageMapEntry)
    - [TestMap.Int32ToSfixed32MapEntry](#json_test-TestMap-Int32ToSfixed32MapEntry)
    - [TestMap.Int32ToSfixed64MapEntry](#json_test-TestMap-Int32ToSfixed64MapEntry)
    - [TestMap.Int32ToSint32MapEntry](#json_test-TestMap-Int32ToSint32MapEntry)
    - [TestMap.Int32ToSint64MapEntry](#json_test-TestMap-Int32ToSint64MapEntry)
    - [TestMap.Int32ToStringMapEntry](#json_test-TestMap-Int32ToStringMapEntry)
    - [TestMap.Int32ToUint32MapEntry](#json_test-TestMap-Int32ToUint32MapEntry)
    - [TestMap.Int32ToUint64MapEntry](#json_test-TestMap-Int32ToUint64MapEntry)
    - [TestMap.Int64ToInt32MapEntry](#json_test-TestMap-Int64ToInt32MapEntry)
    - [TestMap.Sfixed32ToInt32MapEntry](#json_test-TestMap-Sfixed32ToInt32MapEntry)
    - [TestMap.Sfixed64ToInt32MapEntry](#json_test-TestMap-Sfixed64ToInt32MapEntry)
    - [TestMap.Sint32ToInt32MapEntry](#json_test-TestMap-Sint32ToInt32MapEntry)
    - [TestMap.Sint64ToInt32MapEntry](#json_test-TestMap-Sint64ToInt32MapEntry)
    - [TestMap.StringToInt32MapEntry](#json_test-TestMap-StringToInt32MapEntry)
    - [TestMap.Uint32ToInt32MapEntry](#json_test-TestMap-Uint32ToInt32MapEntry)
    - [TestMap.Uint64ToInt32MapEntry](#json_test-TestMap-Uint64ToInt32MapEntry)
    - [TestOneof](#json_test-TestOneof)
    - [TestRecursive](#json_test-TestRecursive)
    - [TestStruct](#json_test-TestStruct)
    - [TestTimestamp](#json_test-TestTimestamp)
    - [TestWrappers](#json_test-TestWrappers)
  
    - [TestAllTypes.AliasedEnum](#json_test-TestAllTypes-AliasedEnum)
    - [TestAllTypes.NestedEnum](#json_test-TestAllTypes-NestedEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_util_src_test_proto_com_google_protobuf_util_json_test-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/util/src/test/proto/com/google/protobuf/util/json_test.proto



<a name="json_test-TestAllTypes"></a>

### TestAllTypes



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) |  |  |
| optional_int64 | [int64](#int64) |  |  |
| optional_uint32 | [uint32](#uint32) |  |  |
| optional_uint64 | [uint64](#uint64) |  |  |
| optional_sint32 | [sint32](#sint32) |  |  |
| optional_sint64 | [sint64](#sint64) |  |  |
| optional_fixed32 | [fixed32](#fixed32) |  |  |
| optional_fixed64 | [fixed64](#fixed64) |  |  |
| optional_sfixed32 | [sfixed32](#sfixed32) |  |  |
| optional_sfixed64 | [sfixed64](#sfixed64) |  |  |
| optional_float | [float](#float) |  |  |
| optional_double | [double](#double) |  |  |
| optional_bool | [bool](#bool) |  |  |
| optional_string | [string](#string) |  |  |
| optional_bytes | [bytes](#bytes) |  |  |
| optional_nested_message | [TestAllTypes.NestedMessage](#json_test-TestAllTypes-NestedMessage) |  |  |
| optional_nested_enum | [TestAllTypes.NestedEnum](#json_test-TestAllTypes-NestedEnum) |  |  |
| optional_aliased_enum | [TestAllTypes.AliasedEnum](#json_test-TestAllTypes-AliasedEnum) |  |  |
| repeated_int32 | [int32](#int32) | repeated | Repeated |
| repeated_int64 | [int64](#int64) | repeated |  |
| repeated_uint32 | [uint32](#uint32) | repeated |  |
| repeated_uint64 | [uint64](#uint64) | repeated |  |
| repeated_sint32 | [sint32](#sint32) | repeated |  |
| repeated_sint64 | [sint64](#sint64) | repeated |  |
| repeated_fixed32 | [fixed32](#fixed32) | repeated |  |
| repeated_fixed64 | [fixed64](#fixed64) | repeated |  |
| repeated_sfixed32 | [sfixed32](#sfixed32) | repeated |  |
| repeated_sfixed64 | [sfixed64](#sfixed64) | repeated |  |
| repeated_float | [float](#float) | repeated |  |
| repeated_double | [double](#double) | repeated |  |
| repeated_bool | [bool](#bool) | repeated |  |
| repeated_string | [string](#string) | repeated |  |
| repeated_bytes | [bytes](#bytes) | repeated |  |
| repeated_nested_message | [TestAllTypes.NestedMessage](#json_test-TestAllTypes-NestedMessage) | repeated |  |
| repeated_nested_enum | [TestAllTypes.NestedEnum](#json_test-TestAllTypes-NestedEnum) | repeated |  |






<a name="json_test-TestAllTypes-NestedMessage"></a>

### TestAllTypes.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) |  |  |






<a name="json_test-TestAny"></a>

### TestAny



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| any_value | [google.protobuf.Any](#google-protobuf-Any) |  |  |
| any_map | [TestAny.AnyMapEntry](#json_test-TestAny-AnyMapEntry) | repeated |  |






<a name="json_test-TestAny-AnyMapEntry"></a>

### TestAny.AnyMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [google.protobuf.Any](#google-protobuf-Any) |  |  |






<a name="json_test-TestCustomJsonName"></a>

### TestCustomJsonName



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) |  |  |






<a name="json_test-TestDuration"></a>

### TestDuration



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| duration_value | [google.protobuf.Duration](#google-protobuf-Duration) |  |  |






<a name="json_test-TestFieldMask"></a>

### TestFieldMask



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_mask_value | [google.protobuf.FieldMask](#google-protobuf-FieldMask) |  |  |






<a name="json_test-TestMap"></a>

### TestMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| int32_to_int32_map | [TestMap.Int32ToInt32MapEntry](#json_test-TestMap-Int32ToInt32MapEntry) | repeated | Instead of testing all combinations (too many), we only make sure all valid types have been used at least in one field as key and in one field as value. |
| int64_to_int32_map | [TestMap.Int64ToInt32MapEntry](#json_test-TestMap-Int64ToInt32MapEntry) | repeated |  |
| uint32_to_int32_map | [TestMap.Uint32ToInt32MapEntry](#json_test-TestMap-Uint32ToInt32MapEntry) | repeated |  |
| uint64_to_int32_map | [TestMap.Uint64ToInt32MapEntry](#json_test-TestMap-Uint64ToInt32MapEntry) | repeated |  |
| sint32_to_int32_map | [TestMap.Sint32ToInt32MapEntry](#json_test-TestMap-Sint32ToInt32MapEntry) | repeated |  |
| sint64_to_int32_map | [TestMap.Sint64ToInt32MapEntry](#json_test-TestMap-Sint64ToInt32MapEntry) | repeated |  |
| fixed32_to_int32_map | [TestMap.Fixed32ToInt32MapEntry](#json_test-TestMap-Fixed32ToInt32MapEntry) | repeated |  |
| fixed64_to_int32_map | [TestMap.Fixed64ToInt32MapEntry](#json_test-TestMap-Fixed64ToInt32MapEntry) | repeated |  |
| sfixed32_to_int32_map | [TestMap.Sfixed32ToInt32MapEntry](#json_test-TestMap-Sfixed32ToInt32MapEntry) | repeated |  |
| sfixed64_to_int32_map | [TestMap.Sfixed64ToInt32MapEntry](#json_test-TestMap-Sfixed64ToInt32MapEntry) | repeated |  |
| bool_to_int32_map | [TestMap.BoolToInt32MapEntry](#json_test-TestMap-BoolToInt32MapEntry) | repeated |  |
| string_to_int32_map | [TestMap.StringToInt32MapEntry](#json_test-TestMap-StringToInt32MapEntry) | repeated |  |
| int32_to_int64_map | [TestMap.Int32ToInt64MapEntry](#json_test-TestMap-Int32ToInt64MapEntry) | repeated |  |
| int32_to_uint32_map | [TestMap.Int32ToUint32MapEntry](#json_test-TestMap-Int32ToUint32MapEntry) | repeated |  |
| int32_to_uint64_map | [TestMap.Int32ToUint64MapEntry](#json_test-TestMap-Int32ToUint64MapEntry) | repeated |  |
| int32_to_sint32_map | [TestMap.Int32ToSint32MapEntry](#json_test-TestMap-Int32ToSint32MapEntry) | repeated |  |
| int32_to_sint64_map | [TestMap.Int32ToSint64MapEntry](#json_test-TestMap-Int32ToSint64MapEntry) | repeated |  |
| int32_to_fixed32_map | [TestMap.Int32ToFixed32MapEntry](#json_test-TestMap-Int32ToFixed32MapEntry) | repeated |  |
| int32_to_fixed64_map | [TestMap.Int32ToFixed64MapEntry](#json_test-TestMap-Int32ToFixed64MapEntry) | repeated |  |
| int32_to_sfixed32_map | [TestMap.Int32ToSfixed32MapEntry](#json_test-TestMap-Int32ToSfixed32MapEntry) | repeated |  |
| int32_to_sfixed64_map | [TestMap.Int32ToSfixed64MapEntry](#json_test-TestMap-Int32ToSfixed64MapEntry) | repeated |  |
| int32_to_float_map | [TestMap.Int32ToFloatMapEntry](#json_test-TestMap-Int32ToFloatMapEntry) | repeated |  |
| int32_to_double_map | [TestMap.Int32ToDoubleMapEntry](#json_test-TestMap-Int32ToDoubleMapEntry) | repeated |  |
| int32_to_bool_map | [TestMap.Int32ToBoolMapEntry](#json_test-TestMap-Int32ToBoolMapEntry) | repeated |  |
| int32_to_string_map | [TestMap.Int32ToStringMapEntry](#json_test-TestMap-Int32ToStringMapEntry) | repeated |  |
| int32_to_bytes_map | [TestMap.Int32ToBytesMapEntry](#json_test-TestMap-Int32ToBytesMapEntry) | repeated |  |
| int32_to_message_map | [TestMap.Int32ToMessageMapEntry](#json_test-TestMap-Int32ToMessageMapEntry) | repeated |  |
| int32_to_enum_map | [TestMap.Int32ToEnumMapEntry](#json_test-TestMap-Int32ToEnumMapEntry) | repeated |  |






<a name="json_test-TestMap-BoolToInt32MapEntry"></a>

### TestMap.BoolToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Fixed32ToInt32MapEntry"></a>

### TestMap.Fixed32ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Fixed64ToInt32MapEntry"></a>

### TestMap.Fixed64ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Int32ToBoolMapEntry"></a>

### TestMap.Int32ToBoolMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bool](#bool) |  |  |






<a name="json_test-TestMap-Int32ToBytesMapEntry"></a>

### TestMap.Int32ToBytesMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="json_test-TestMap-Int32ToDoubleMapEntry"></a>

### TestMap.Int32ToDoubleMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [double](#double) |  |  |






<a name="json_test-TestMap-Int32ToEnumMapEntry"></a>

### TestMap.Int32ToEnumMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestAllTypes.NestedEnum](#json_test-TestAllTypes-NestedEnum) |  |  |






<a name="json_test-TestMap-Int32ToFixed32MapEntry"></a>

### TestMap.Int32ToFixed32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="json_test-TestMap-Int32ToFixed64MapEntry"></a>

### TestMap.Int32ToFixed64MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="json_test-TestMap-Int32ToFloatMapEntry"></a>

### TestMap.Int32ToFloatMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [float](#float) |  |  |






<a name="json_test-TestMap-Int32ToInt32MapEntry"></a>

### TestMap.Int32ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Int32ToInt64MapEntry"></a>

### TestMap.Int32ToInt64MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int64](#int64) |  |  |






<a name="json_test-TestMap-Int32ToMessageMapEntry"></a>

### TestMap.Int32ToMessageMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestAllTypes.NestedMessage](#json_test-TestAllTypes-NestedMessage) |  |  |






<a name="json_test-TestMap-Int32ToSfixed32MapEntry"></a>

### TestMap.Int32ToSfixed32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="json_test-TestMap-Int32ToSfixed64MapEntry"></a>

### TestMap.Int32ToSfixed64MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="json_test-TestMap-Int32ToSint32MapEntry"></a>

### TestMap.Int32ToSint32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="json_test-TestMap-Int32ToSint64MapEntry"></a>

### TestMap.Int32ToSint64MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="json_test-TestMap-Int32ToStringMapEntry"></a>

### TestMap.Int32ToStringMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [string](#string) |  |  |






<a name="json_test-TestMap-Int32ToUint32MapEntry"></a>

### TestMap.Int32ToUint32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="json_test-TestMap-Int32ToUint64MapEntry"></a>

### TestMap.Int32ToUint64MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="json_test-TestMap-Int64ToInt32MapEntry"></a>

### TestMap.Int64ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Sfixed32ToInt32MapEntry"></a>

### TestMap.Sfixed32ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Sfixed64ToInt32MapEntry"></a>

### TestMap.Sfixed64ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Sint32ToInt32MapEntry"></a>

### TestMap.Sint32ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Sint64ToInt32MapEntry"></a>

### TestMap.Sint64ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-StringToInt32MapEntry"></a>

### TestMap.StringToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Uint32ToInt32MapEntry"></a>

### TestMap.Uint32ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestMap-Uint64ToInt32MapEntry"></a>

### TestMap.Uint64ToInt32MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [int32](#int32) |  |  |






<a name="json_test-TestOneof"></a>

### TestOneof



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| oneof_int32 | [int32](#int32) |  |  |
| oneof_nested_message | [TestAllTypes.NestedMessage](#json_test-TestAllTypes-NestedMessage) |  |  |
| oneof_null_value | [google.protobuf.NullValue](#google-protobuf-NullValue) |  |  |






<a name="json_test-TestRecursive"></a>

### TestRecursive



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) |  |  |
| nested | [TestRecursive](#json_test-TestRecursive) |  |  |






<a name="json_test-TestStruct"></a>

### TestStruct



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| struct_value | [google.protobuf.Struct](#google-protobuf-Struct) |  |  |
| value | [google.protobuf.Value](#google-protobuf-Value) |  |  |
| list_value | [google.protobuf.ListValue](#google-protobuf-ListValue) |  |  |






<a name="json_test-TestTimestamp"></a>

### TestTimestamp



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| timestamp_value | [google.protobuf.Timestamp](#google-protobuf-Timestamp) |  |  |






<a name="json_test-TestWrappers"></a>

### TestWrappers



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| int32_value | [google.protobuf.Int32Value](#google-protobuf-Int32Value) |  |  |
| uint32_value | [google.protobuf.UInt32Value](#google-protobuf-UInt32Value) |  |  |
| int64_value | [google.protobuf.Int64Value](#google-protobuf-Int64Value) |  |  |
| uint64_value | [google.protobuf.UInt64Value](#google-protobuf-UInt64Value) |  |  |
| float_value | [google.protobuf.FloatValue](#google-protobuf-FloatValue) |  |  |
| double_value | [google.protobuf.DoubleValue](#google-protobuf-DoubleValue) |  |  |
| bool_value | [google.protobuf.BoolValue](#google-protobuf-BoolValue) |  |  |
| string_value | [google.protobuf.StringValue](#google-protobuf-StringValue) |  |  |
| bytes_value | [google.protobuf.BytesValue](#google-protobuf-BytesValue) |  |  |





 


<a name="json_test-TestAllTypes-AliasedEnum"></a>

### TestAllTypes.AliasedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ALIAS_FOO | 0 |  |
| ALIAS_BAR | 1 |  |
| ALIAS_BAZ | 2 |  |
| QUX | 2 |  |
| qux | 2 |  |
| bAz | 2 |  |



<a name="json_test-TestAllTypes-NestedEnum"></a>

### TestAllTypes.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |
| BAR | 1 |  |
| BAZ | 2 |  |


 

 

 



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

