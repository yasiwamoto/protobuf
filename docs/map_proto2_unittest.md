# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/map_proto2_unittest.proto](#objectivec_Tests_map_proto2_unittest-proto)
    - [TestEnumMap](#objc-protobuf-tests-TestEnumMap)
    - [TestEnumMap.KnownMapFieldEntry](#objc-protobuf-tests-TestEnumMap-KnownMapFieldEntry)
    - [TestEnumMap.UnknownMapFieldEntry](#objc-protobuf-tests-TestEnumMap-UnknownMapFieldEntry)
    - [TestEnumMapPlusExtra](#objc-protobuf-tests-TestEnumMapPlusExtra)
    - [TestEnumMapPlusExtra.KnownMapFieldEntry](#objc-protobuf-tests-TestEnumMapPlusExtra-KnownMapFieldEntry)
    - [TestEnumMapPlusExtra.UnknownMapFieldEntry](#objc-protobuf-tests-TestEnumMapPlusExtra-UnknownMapFieldEntry)
    - [TestImportEnumMap](#objc-protobuf-tests-TestImportEnumMap)
    - [TestImportEnumMap.ImportEnumAmpEntry](#objc-protobuf-tests-TestImportEnumMap-ImportEnumAmpEntry)
    - [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap)
    - [TestIntIntMap.MEntry](#objc-protobuf-tests-TestIntIntMap-MEntry)
    - [TestMaps](#objc-protobuf-tests-TestMaps)
    - [TestMaps.MBoolEntry](#objc-protobuf-tests-TestMaps-MBoolEntry)
    - [TestMaps.MFixed32Entry](#objc-protobuf-tests-TestMaps-MFixed32Entry)
    - [TestMaps.MFixed64Entry](#objc-protobuf-tests-TestMaps-MFixed64Entry)
    - [TestMaps.MInt32Entry](#objc-protobuf-tests-TestMaps-MInt32Entry)
    - [TestMaps.MInt64Entry](#objc-protobuf-tests-TestMaps-MInt64Entry)
    - [TestMaps.MSfixed32Entry](#objc-protobuf-tests-TestMaps-MSfixed32Entry)
    - [TestMaps.MSfixed64Entry](#objc-protobuf-tests-TestMaps-MSfixed64Entry)
    - [TestMaps.MSint32Entry](#objc-protobuf-tests-TestMaps-MSint32Entry)
    - [TestMaps.MSint64Entry](#objc-protobuf-tests-TestMaps-MSint64Entry)
    - [TestMaps.MStringEntry](#objc-protobuf-tests-TestMaps-MStringEntry)
    - [TestMaps.MUint32Entry](#objc-protobuf-tests-TestMaps-MUint32Entry)
    - [TestMaps.MUint64Entry](#objc-protobuf-tests-TestMaps-MUint64Entry)
    - [TestSubmessageMaps](#objc-protobuf-tests-TestSubmessageMaps)
  
    - [Proto2MapEnum](#objc-protobuf-tests-Proto2MapEnum)
    - [Proto2MapEnumPlusExtra](#objc-protobuf-tests-Proto2MapEnumPlusExtra)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_map_proto2_unittest-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/map_proto2_unittest.proto



<a name="objc-protobuf-tests-TestEnumMap"></a>

### TestEnumMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| known_map_field | [TestEnumMap.KnownMapFieldEntry](#objc-protobuf-tests-TestEnumMap-KnownMapFieldEntry) | repeated |  |
| unknown_map_field | [TestEnumMap.UnknownMapFieldEntry](#objc-protobuf-tests-TestEnumMap-UnknownMapFieldEntry) | repeated |  |






<a name="objc-protobuf-tests-TestEnumMap-KnownMapFieldEntry"></a>

### TestEnumMap.KnownMapFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2MapEnum](#objc-protobuf-tests-Proto2MapEnum) | optional |  |






<a name="objc-protobuf-tests-TestEnumMap-UnknownMapFieldEntry"></a>

### TestEnumMap.UnknownMapFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2MapEnum](#objc-protobuf-tests-Proto2MapEnum) | optional |  |






<a name="objc-protobuf-tests-TestEnumMapPlusExtra"></a>

### TestEnumMapPlusExtra



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| known_map_field | [TestEnumMapPlusExtra.KnownMapFieldEntry](#objc-protobuf-tests-TestEnumMapPlusExtra-KnownMapFieldEntry) | repeated |  |
| unknown_map_field | [TestEnumMapPlusExtra.UnknownMapFieldEntry](#objc-protobuf-tests-TestEnumMapPlusExtra-UnknownMapFieldEntry) | repeated |  |






<a name="objc-protobuf-tests-TestEnumMapPlusExtra-KnownMapFieldEntry"></a>

### TestEnumMapPlusExtra.KnownMapFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2MapEnumPlusExtra](#objc-protobuf-tests-Proto2MapEnumPlusExtra) | optional |  |






<a name="objc-protobuf-tests-TestEnumMapPlusExtra-UnknownMapFieldEntry"></a>

### TestEnumMapPlusExtra.UnknownMapFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2MapEnumPlusExtra](#objc-protobuf-tests-Proto2MapEnumPlusExtra) | optional |  |






<a name="objc-protobuf-tests-TestImportEnumMap"></a>

### TestImportEnumMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| import_enum_amp | [TestImportEnumMap.ImportEnumAmpEntry](#objc-protobuf-tests-TestImportEnumMap-ImportEnumAmpEntry) | repeated |  |






<a name="objc-protobuf-tests-TestImportEnumMap-ImportEnumAmpEntry"></a>

### TestImportEnumMap.ImportEnumAmpEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [import.EnumForMap](#objc-protobuf-tests-import-EnumForMap) | optional |  |






<a name="objc-protobuf-tests-TestIntIntMap"></a>

### TestIntIntMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| m | [TestIntIntMap.MEntry](#objc-protobuf-tests-TestIntIntMap-MEntry) | repeated |  |






<a name="objc-protobuf-tests-TestIntIntMap-MEntry"></a>

### TestIntIntMap.MEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestMaps"></a>

### TestMaps
Test all key types: string, plus the non-floating-point scalars.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| m_int32 | [TestMaps.MInt32Entry](#objc-protobuf-tests-TestMaps-MInt32Entry) | repeated |  |
| m_int64 | [TestMaps.MInt64Entry](#objc-protobuf-tests-TestMaps-MInt64Entry) | repeated |  |
| m_uint32 | [TestMaps.MUint32Entry](#objc-protobuf-tests-TestMaps-MUint32Entry) | repeated |  |
| m_uint64 | [TestMaps.MUint64Entry](#objc-protobuf-tests-TestMaps-MUint64Entry) | repeated |  |
| m_sint32 | [TestMaps.MSint32Entry](#objc-protobuf-tests-TestMaps-MSint32Entry) | repeated |  |
| m_sint64 | [TestMaps.MSint64Entry](#objc-protobuf-tests-TestMaps-MSint64Entry) | repeated |  |
| m_fixed32 | [TestMaps.MFixed32Entry](#objc-protobuf-tests-TestMaps-MFixed32Entry) | repeated |  |
| m_fixed64 | [TestMaps.MFixed64Entry](#objc-protobuf-tests-TestMaps-MFixed64Entry) | repeated |  |
| m_sfixed32 | [TestMaps.MSfixed32Entry](#objc-protobuf-tests-TestMaps-MSfixed32Entry) | repeated |  |
| m_sfixed64 | [TestMaps.MSfixed64Entry](#objc-protobuf-tests-TestMaps-MSfixed64Entry) | repeated |  |
| m_bool | [TestMaps.MBoolEntry](#objc-protobuf-tests-TestMaps-MBoolEntry) | repeated |  |
| m_string | [TestMaps.MStringEntry](#objc-protobuf-tests-TestMaps-MStringEntry) | repeated |  |






<a name="objc-protobuf-tests-TestMaps-MBoolEntry"></a>

### TestMaps.MBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MFixed32Entry"></a>

### TestMaps.MFixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MFixed64Entry"></a>

### TestMaps.MFixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MInt32Entry"></a>

### TestMaps.MInt32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MInt64Entry"></a>

### TestMaps.MInt64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MSfixed32Entry"></a>

### TestMaps.MSfixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MSfixed64Entry"></a>

### TestMaps.MSfixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MSint32Entry"></a>

### TestMaps.MSint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MSint64Entry"></a>

### TestMaps.MSint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MStringEntry"></a>

### TestMaps.MStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MUint32Entry"></a>

### TestMaps.MUint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestMaps-MUint64Entry"></a>

### TestMaps.MUint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [TestIntIntMap](#objc-protobuf-tests-TestIntIntMap) | optional |  |






<a name="objc-protobuf-tests-TestSubmessageMaps"></a>

### TestSubmessageMaps
Test maps in submessages.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| m | [TestMaps](#objc-protobuf-tests-TestMaps) | optional |  |





 


<a name="objc-protobuf-tests-Proto2MapEnum"></a>

### Proto2MapEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| PROTO2_MAP_ENUM_FOO | 0 |  |
| PROTO2_MAP_ENUM_BAR | 1 |  |
| PROTO2_MAP_ENUM_BAZ | 2 |  |



<a name="objc-protobuf-tests-Proto2MapEnumPlusExtra"></a>

### Proto2MapEnumPlusExtra


| Name | Number | Description |
| ---- | ------ | ----------- |
| E_PROTO2_MAP_ENUM_FOO | 0 |  |
| E_PROTO2_MAP_ENUM_BAR | 1 |  |
| E_PROTO2_MAP_ENUM_BAZ | 2 |  |
| E_PROTO2_MAP_ENUM_EXTRA | 3 |  |


 

 

 



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

