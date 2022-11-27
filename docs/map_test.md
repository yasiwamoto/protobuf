# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/core/src/test/proto/com/google/protobuf/map_test.proto](#java_core_src_test_proto_com_google_protobuf_map_test-proto)
    - [BizarroTestMap](#map_test-BizarroTestMap)
    - [BizarroTestMap.Int32ToBytesFieldEntry](#map_test-BizarroTestMap-Int32ToBytesFieldEntry)
    - [BizarroTestMap.Int32ToEnumFieldEntry](#map_test-BizarroTestMap-Int32ToEnumFieldEntry)
    - [BizarroTestMap.Int32ToInt32FieldEntry](#map_test-BizarroTestMap-Int32ToInt32FieldEntry)
    - [BizarroTestMap.Int32ToMessageFieldEntry](#map_test-BizarroTestMap-Int32ToMessageFieldEntry)
    - [BizarroTestMap.Int32ToStringFieldEntry](#map_test-BizarroTestMap-Int32ToStringFieldEntry)
    - [BizarroTestMap.StringToInt32FieldEntry](#map_test-BizarroTestMap-StringToInt32FieldEntry)
    - [MapContainer](#map_test-MapContainer)
    - [MapContainer.MyMapEntry](#map_test-MapContainer-MyMapEntry)
    - [ReservedAsMapField](#map_test-ReservedAsMapField)
    - [ReservedAsMapField.ClassEntry](#map_test-ReservedAsMapField-ClassEntry)
    - [ReservedAsMapField.ConstEntry](#map_test-ReservedAsMapField-ConstEntry)
    - [ReservedAsMapField.EnumEntry](#map_test-ReservedAsMapField-EnumEntry)
    - [ReservedAsMapField.IfEntry](#map_test-ReservedAsMapField-IfEntry)
    - [ReservedAsMapField.IntEntry](#map_test-ReservedAsMapField-IntEntry)
    - [ReservedAsMapField.NullEntry](#map_test-ReservedAsMapField-NullEntry)
    - [ReservedAsMapField.PackageEntry](#map_test-ReservedAsMapField-PackageEntry)
    - [ReservedAsMapField.PrivateEntry](#map_test-ReservedAsMapField-PrivateEntry)
    - [ReservedAsMapField.StringEntry](#map_test-ReservedAsMapField-StringEntry)
    - [ReservedAsMapField.VoidEntry](#map_test-ReservedAsMapField-VoidEntry)
    - [ReservedAsMapFieldWithEnumValue](#map_test-ReservedAsMapFieldWithEnumValue)
    - [ReservedAsMapFieldWithEnumValue.ClassEntry](#map_test-ReservedAsMapFieldWithEnumValue-ClassEntry)
    - [ReservedAsMapFieldWithEnumValue.ConstEntry](#map_test-ReservedAsMapFieldWithEnumValue-ConstEntry)
    - [ReservedAsMapFieldWithEnumValue.EnumEntry](#map_test-ReservedAsMapFieldWithEnumValue-EnumEntry)
    - [ReservedAsMapFieldWithEnumValue.IfEntry](#map_test-ReservedAsMapFieldWithEnumValue-IfEntry)
    - [ReservedAsMapFieldWithEnumValue.IntEntry](#map_test-ReservedAsMapFieldWithEnumValue-IntEntry)
    - [ReservedAsMapFieldWithEnumValue.NullEntry](#map_test-ReservedAsMapFieldWithEnumValue-NullEntry)
    - [ReservedAsMapFieldWithEnumValue.PackageEntry](#map_test-ReservedAsMapFieldWithEnumValue-PackageEntry)
    - [ReservedAsMapFieldWithEnumValue.PrivateEntry](#map_test-ReservedAsMapFieldWithEnumValue-PrivateEntry)
    - [ReservedAsMapFieldWithEnumValue.StringEntry](#map_test-ReservedAsMapFieldWithEnumValue-StringEntry)
    - [ReservedAsMapFieldWithEnumValue.VoidEntry](#map_test-ReservedAsMapFieldWithEnumValue-VoidEntry)
    - [TestMap](#map_test-TestMap)
    - [TestMap.Int32ToBytesFieldEntry](#map_test-TestMap-Int32ToBytesFieldEntry)
    - [TestMap.Int32ToEnumFieldEntry](#map_test-TestMap-Int32ToEnumFieldEntry)
    - [TestMap.Int32ToInt32FieldEntry](#map_test-TestMap-Int32ToInt32FieldEntry)
    - [TestMap.Int32ToMessageFieldEntry](#map_test-TestMap-Int32ToMessageFieldEntry)
    - [TestMap.Int32ToStringFieldEntry](#map_test-TestMap-Int32ToStringFieldEntry)
    - [TestMap.Int64ToInt32FieldEntry](#map_test-TestMap-Int64ToInt32FieldEntry)
    - [TestMap.MessageValue](#map_test-TestMap-MessageValue)
    - [TestMap.StringToInt32FieldEntry](#map_test-TestMap-StringToInt32FieldEntry)
    - [TestMap.Uint32ToInt32FieldEntry](#map_test-TestMap-Uint32ToInt32FieldEntry)
    - [TestOnChangeEventPropagation](#map_test-TestOnChangeEventPropagation)
  
    - [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum)
    - [TestMap.EnumValue](#map_test-TestMap-EnumValue)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_core_src_test_proto_com_google_protobuf_map_test-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/core/src/test/proto/com/google/protobuf/map_test.proto



<a name="map_test-BizarroTestMap"></a>

### BizarroTestMap
a decoy of TestMap for testing parsing errors


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| int32_to_int32_field | [BizarroTestMap.Int32ToInt32FieldEntry](#map_test-BizarroTestMap-Int32ToInt32FieldEntry) | repeated | same key type, different value |
| int32_to_string_field | [BizarroTestMap.Int32ToStringFieldEntry](#map_test-BizarroTestMap-Int32ToStringFieldEntry) | repeated | different key and value types |
| int32_to_bytes_field | [BizarroTestMap.Int32ToBytesFieldEntry](#map_test-BizarroTestMap-Int32ToBytesFieldEntry) | repeated | different key types, same value |
| int32_to_enum_field | [BizarroTestMap.Int32ToEnumFieldEntry](#map_test-BizarroTestMap-Int32ToEnumFieldEntry) | repeated | different key and value types |
| int32_to_message_field | [BizarroTestMap.Int32ToMessageFieldEntry](#map_test-BizarroTestMap-Int32ToMessageFieldEntry) | repeated | different key and value types |
| string_to_int32_field | [BizarroTestMap.StringToInt32FieldEntry](#map_test-BizarroTestMap-StringToInt32FieldEntry) | repeated | same key type, different value |






<a name="map_test-BizarroTestMap-Int32ToBytesFieldEntry"></a>

### BizarroTestMap.Int32ToBytesFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="map_test-BizarroTestMap-Int32ToEnumFieldEntry"></a>

### BizarroTestMap.Int32ToEnumFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="map_test-BizarroTestMap-Int32ToInt32FieldEntry"></a>

### BizarroTestMap.Int32ToInt32FieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="map_test-BizarroTestMap-Int32ToMessageFieldEntry"></a>

### BizarroTestMap.Int32ToMessageFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="map_test-BizarroTestMap-Int32ToStringFieldEntry"></a>

### BizarroTestMap.Int32ToStringFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="map_test-BizarroTestMap-StringToInt32FieldEntry"></a>

### BizarroTestMap.StringToInt32FieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="map_test-MapContainer"></a>

### MapContainer
https://github.com/protocolbuffers/protobuf/issues/9785


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| my_map | [MapContainer.MyMapEntry](#map_test-MapContainer-MyMapEntry) | repeated |  |






<a name="map_test-MapContainer-MyMapEntry"></a>

### MapContainer.MyMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="map_test-ReservedAsMapField"></a>

### ReservedAsMapField
Used to test that java reserved words can be used as protobuf field names
Not all reserved words are tested (to avoid bloat) but instead an arbitrary
subset of them chosen to cover various keyword categories like
type, modifier, declaration, etc.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| if | [ReservedAsMapField.IfEntry](#map_test-ReservedAsMapField-IfEntry) | repeated |  |
| const | [ReservedAsMapField.ConstEntry](#map_test-ReservedAsMapField-ConstEntry) | repeated |  |
| private | [ReservedAsMapField.PrivateEntry](#map_test-ReservedAsMapField-PrivateEntry) | repeated |  |
| class | [ReservedAsMapField.ClassEntry](#map_test-ReservedAsMapField-ClassEntry) | repeated |  |
| int | [ReservedAsMapField.IntEntry](#map_test-ReservedAsMapField-IntEntry) | repeated |  |
| void | [ReservedAsMapField.VoidEntry](#map_test-ReservedAsMapField-VoidEntry) | repeated |  |
| string | [ReservedAsMapField.StringEntry](#map_test-ReservedAsMapField-StringEntry) | repeated | These are also proto keywords |
| package | [ReservedAsMapField.PackageEntry](#map_test-ReservedAsMapField-PackageEntry) | repeated |  |
| enum | [ReservedAsMapField.EnumEntry](#map_test-ReservedAsMapField-EnumEntry) | repeated | Most recent Java reserved word |
| null | [ReservedAsMapField.NullEntry](#map_test-ReservedAsMapField-NullEntry) | repeated | null is not a &#39;reserved word&#39; per se but as a literal needs similar care |






<a name="map_test-ReservedAsMapField-ClassEntry"></a>

### ReservedAsMapField.ClassEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-ConstEntry"></a>

### ReservedAsMapField.ConstEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-EnumEntry"></a>

### ReservedAsMapField.EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-IfEntry"></a>

### ReservedAsMapField.IfEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-IntEntry"></a>

### ReservedAsMapField.IntEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-NullEntry"></a>

### ReservedAsMapField.NullEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-PackageEntry"></a>

### ReservedAsMapField.PackageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-PrivateEntry"></a>

### ReservedAsMapField.PrivateEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-StringEntry"></a>

### ReservedAsMapField.StringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapField-VoidEntry"></a>

### ReservedAsMapField.VoidEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue"></a>

### ReservedAsMapFieldWithEnumValue



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| if | [ReservedAsMapFieldWithEnumValue.IfEntry](#map_test-ReservedAsMapFieldWithEnumValue-IfEntry) | repeated |  |
| const | [ReservedAsMapFieldWithEnumValue.ConstEntry](#map_test-ReservedAsMapFieldWithEnumValue-ConstEntry) | repeated |  |
| private | [ReservedAsMapFieldWithEnumValue.PrivateEntry](#map_test-ReservedAsMapFieldWithEnumValue-PrivateEntry) | repeated |  |
| class | [ReservedAsMapFieldWithEnumValue.ClassEntry](#map_test-ReservedAsMapFieldWithEnumValue-ClassEntry) | repeated |  |
| int | [ReservedAsMapFieldWithEnumValue.IntEntry](#map_test-ReservedAsMapFieldWithEnumValue-IntEntry) | repeated |  |
| void | [ReservedAsMapFieldWithEnumValue.VoidEntry](#map_test-ReservedAsMapFieldWithEnumValue-VoidEntry) | repeated |  |
| string | [ReservedAsMapFieldWithEnumValue.StringEntry](#map_test-ReservedAsMapFieldWithEnumValue-StringEntry) | repeated | These are also proto keywords |
| package | [ReservedAsMapFieldWithEnumValue.PackageEntry](#map_test-ReservedAsMapFieldWithEnumValue-PackageEntry) | repeated |  |
| enum | [ReservedAsMapFieldWithEnumValue.EnumEntry](#map_test-ReservedAsMapFieldWithEnumValue-EnumEntry) | repeated | Most recent Java reserved word |
| null | [ReservedAsMapFieldWithEnumValue.NullEntry](#map_test-ReservedAsMapFieldWithEnumValue-NullEntry) | repeated | null is not a &#39;reserved word&#39; per se but as a literal needs similar care |






<a name="map_test-ReservedAsMapFieldWithEnumValue-ClassEntry"></a>

### ReservedAsMapFieldWithEnumValue.ClassEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-ConstEntry"></a>

### ReservedAsMapFieldWithEnumValue.ConstEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-EnumEntry"></a>

### ReservedAsMapFieldWithEnumValue.EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-IfEntry"></a>

### ReservedAsMapFieldWithEnumValue.IfEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-IntEntry"></a>

### ReservedAsMapFieldWithEnumValue.IntEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-NullEntry"></a>

### ReservedAsMapFieldWithEnumValue.NullEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-PackageEntry"></a>

### ReservedAsMapFieldWithEnumValue.PackageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-PrivateEntry"></a>

### ReservedAsMapFieldWithEnumValue.PrivateEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-StringEntry"></a>

### ReservedAsMapFieldWithEnumValue.StringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-ReservedAsMapFieldWithEnumValue-VoidEntry"></a>

### ReservedAsMapFieldWithEnumValue.VoidEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ReservedAsMapFieldWithEnumValue.SampleEnum](#map_test-ReservedAsMapFieldWithEnumValue-SampleEnum) |  |  |






<a name="map_test-TestMap"></a>

### TestMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| int32_to_int32_field | [TestMap.Int32ToInt32FieldEntry](#map_test-TestMap-Int32ToInt32FieldEntry) | repeated |  |
| int32_to_string_field | [TestMap.Int32ToStringFieldEntry](#map_test-TestMap-Int32ToStringFieldEntry) | repeated |  |
| int32_to_bytes_field | [TestMap.Int32ToBytesFieldEntry](#map_test-TestMap-Int32ToBytesFieldEntry) | repeated |  |
| int32_to_enum_field | [TestMap.Int32ToEnumFieldEntry](#map_test-TestMap-Int32ToEnumFieldEntry) | repeated |  |
| int32_to_message_field | [TestMap.Int32ToMessageFieldEntry](#map_test-TestMap-Int32ToMessageFieldEntry) | repeated |  |
| string_to_int32_field | [TestMap.StringToInt32FieldEntry](#map_test-TestMap-StringToInt32FieldEntry) | repeated |  |
| uint32_to_int32_field | [TestMap.Uint32ToInt32FieldEntry](#map_test-TestMap-Uint32ToInt32FieldEntry) | repeated |  |
| int64_to_int32_field | [TestMap.Int64ToInt32FieldEntry](#map_test-TestMap-Int64ToInt32FieldEntry) | repeated |  |






<a name="map_test-TestMap-Int32ToBytesFieldEntry"></a>

### TestMap.Int32ToBytesFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="map_test-TestMap-Int32ToEnumFieldEntry"></a>

### TestMap.Int32ToEnumFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestMap.EnumValue](#map_test-TestMap-EnumValue) |  |  |






<a name="map_test-TestMap-Int32ToInt32FieldEntry"></a>

### TestMap.Int32ToInt32FieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="map_test-TestMap-Int32ToMessageFieldEntry"></a>

### TestMap.Int32ToMessageFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestMap.MessageValue](#map_test-TestMap-MessageValue) |  |  |






<a name="map_test-TestMap-Int32ToStringFieldEntry"></a>

### TestMap.Int32ToStringFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [string](#string) |  |  |






<a name="map_test-TestMap-Int64ToInt32FieldEntry"></a>

### TestMap.Int64ToInt32FieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int32](#int32) |  |  |






<a name="map_test-TestMap-MessageValue"></a>

### TestMap.MessageValue



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) |  |  |






<a name="map_test-TestMap-StringToInt32FieldEntry"></a>

### TestMap.StringToInt32FieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="map_test-TestMap-Uint32ToInt32FieldEntry"></a>

### TestMap.Uint32ToInt32FieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [int32](#int32) |  |  |






<a name="map_test-TestOnChangeEventPropagation"></a>

### TestOnChangeEventPropagation
Used to test that a nested builder containing map fields will properly
propagate the onChange event and mark its parent dirty when a change
is made to a map field.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_message | [TestMap](#map_test-TestMap) |  |  |





 


<a name="map_test-ReservedAsMapFieldWithEnumValue-SampleEnum"></a>

### ReservedAsMapFieldWithEnumValue.SampleEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| A | 0 |  |
| B | 1 |  |



<a name="map_test-TestMap-EnumValue"></a>

### TestMap.EnumValue


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |
| BAR | 1 |  |
| BAZ | 2 |  |
| QUX | 3 |  |


 

 

 



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

