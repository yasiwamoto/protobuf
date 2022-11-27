# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/map_unittest.proto](#objectivec_Tests_map_unittest-proto)
    - [MessageContainingEnumCalledType](#objc-protobuf-tests-MessageContainingEnumCalledType)
    - [MessageContainingEnumCalledType.TypeEntry](#objc-protobuf-tests-MessageContainingEnumCalledType-TypeEntry)
    - [MessageContainingMapCalledEntry](#objc-protobuf-tests-MessageContainingMapCalledEntry)
    - [MessageContainingMapCalledEntry.EntryEntry](#objc-protobuf-tests-MessageContainingMapCalledEntry-EntryEntry)
    - [TestArenaMap](#objc-protobuf-tests-TestArenaMap)
    - [TestArenaMap.MapBoolBoolEntry](#objc-protobuf-tests-TestArenaMap-MapBoolBoolEntry)
    - [TestArenaMap.MapFixed32Fixed32Entry](#objc-protobuf-tests-TestArenaMap-MapFixed32Fixed32Entry)
    - [TestArenaMap.MapFixed64Fixed64Entry](#objc-protobuf-tests-TestArenaMap-MapFixed64Fixed64Entry)
    - [TestArenaMap.MapInt32BytesEntry](#objc-protobuf-tests-TestArenaMap-MapInt32BytesEntry)
    - [TestArenaMap.MapInt32DoubleEntry](#objc-protobuf-tests-TestArenaMap-MapInt32DoubleEntry)
    - [TestArenaMap.MapInt32EnumEntry](#objc-protobuf-tests-TestArenaMap-MapInt32EnumEntry)
    - [TestArenaMap.MapInt32FloatEntry](#objc-protobuf-tests-TestArenaMap-MapInt32FloatEntry)
    - [TestArenaMap.MapInt32ForeignMessageEntry](#objc-protobuf-tests-TestArenaMap-MapInt32ForeignMessageEntry)
    - [TestArenaMap.MapInt32Int32Entry](#objc-protobuf-tests-TestArenaMap-MapInt32Int32Entry)
    - [TestArenaMap.MapInt64Int64Entry](#objc-protobuf-tests-TestArenaMap-MapInt64Int64Entry)
    - [TestArenaMap.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-TestArenaMap-MapSfixed32Sfixed32Entry)
    - [TestArenaMap.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-TestArenaMap-MapSfixed64Sfixed64Entry)
    - [TestArenaMap.MapSint32Sint32Entry](#objc-protobuf-tests-TestArenaMap-MapSint32Sint32Entry)
    - [TestArenaMap.MapSint64Sint64Entry](#objc-protobuf-tests-TestArenaMap-MapSint64Sint64Entry)
    - [TestArenaMap.MapStringStringEntry](#objc-protobuf-tests-TestArenaMap-MapStringStringEntry)
    - [TestArenaMap.MapUint32Uint32Entry](#objc-protobuf-tests-TestArenaMap-MapUint32Uint32Entry)
    - [TestArenaMap.MapUint64Uint64Entry](#objc-protobuf-tests-TestArenaMap-MapUint64Uint64Entry)
    - [TestMap](#objc-protobuf-tests-TestMap)
    - [TestMap.MapBoolBoolEntry](#objc-protobuf-tests-TestMap-MapBoolBoolEntry)
    - [TestMap.MapFixed32Fixed32Entry](#objc-protobuf-tests-TestMap-MapFixed32Fixed32Entry)
    - [TestMap.MapFixed64Fixed64Entry](#objc-protobuf-tests-TestMap-MapFixed64Fixed64Entry)
    - [TestMap.MapInt32AllTypesEntry](#objc-protobuf-tests-TestMap-MapInt32AllTypesEntry)
    - [TestMap.MapInt32BytesEntry](#objc-protobuf-tests-TestMap-MapInt32BytesEntry)
    - [TestMap.MapInt32DoubleEntry](#objc-protobuf-tests-TestMap-MapInt32DoubleEntry)
    - [TestMap.MapInt32EnumEntry](#objc-protobuf-tests-TestMap-MapInt32EnumEntry)
    - [TestMap.MapInt32FloatEntry](#objc-protobuf-tests-TestMap-MapInt32FloatEntry)
    - [TestMap.MapInt32ForeignMessageEntry](#objc-protobuf-tests-TestMap-MapInt32ForeignMessageEntry)
    - [TestMap.MapInt32Int32Entry](#objc-protobuf-tests-TestMap-MapInt32Int32Entry)
    - [TestMap.MapInt64Int64Entry](#objc-protobuf-tests-TestMap-MapInt64Int64Entry)
    - [TestMap.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-TestMap-MapSfixed32Sfixed32Entry)
    - [TestMap.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-TestMap-MapSfixed64Sfixed64Entry)
    - [TestMap.MapSint32Sint32Entry](#objc-protobuf-tests-TestMap-MapSint32Sint32Entry)
    - [TestMap.MapSint64Sint64Entry](#objc-protobuf-tests-TestMap-MapSint64Sint64Entry)
    - [TestMap.MapStringForeignMessageEntry](#objc-protobuf-tests-TestMap-MapStringForeignMessageEntry)
    - [TestMap.MapStringStringEntry](#objc-protobuf-tests-TestMap-MapStringStringEntry)
    - [TestMap.MapUint32Uint32Entry](#objc-protobuf-tests-TestMap-MapUint32Uint32Entry)
    - [TestMap.MapUint64Uint64Entry](#objc-protobuf-tests-TestMap-MapUint64Uint64Entry)
    - [TestMapSubmessage](#objc-protobuf-tests-TestMapSubmessage)
    - [TestMessageMap](#objc-protobuf-tests-TestMessageMap)
    - [TestMessageMap.MapInt32MessageEntry](#objc-protobuf-tests-TestMessageMap-MapInt32MessageEntry)
    - [TestRecursiveMapMessage](#objc-protobuf-tests-TestRecursiveMapMessage)
    - [TestRecursiveMapMessage.AEntry](#objc-protobuf-tests-TestRecursiveMapMessage-AEntry)
    - [TestRequiredMessageMap](#objc-protobuf-tests-TestRequiredMessageMap)
    - [TestRequiredMessageMap.MapFieldEntry](#objc-protobuf-tests-TestRequiredMessageMap-MapFieldEntry)
    - [TestSameTypeMap](#objc-protobuf-tests-TestSameTypeMap)
    - [TestSameTypeMap.Map1Entry](#objc-protobuf-tests-TestSameTypeMap-Map1Entry)
    - [TestSameTypeMap.Map2Entry](#objc-protobuf-tests-TestSameTypeMap-Map2Entry)
  
    - [MapEnum](#objc-protobuf-tests-MapEnum)
    - [MessageContainingEnumCalledType.Type](#objc-protobuf-tests-MessageContainingEnumCalledType-Type)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_map_unittest-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/map_unittest.proto



<a name="objc-protobuf-tests-MessageContainingEnumCalledType"></a>

### MessageContainingEnumCalledType
Previously, message containing enum called Type cannot be used as value of
map field.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type | [MessageContainingEnumCalledType.TypeEntry](#objc-protobuf-tests-MessageContainingEnumCalledType-TypeEntry) | repeated |  |






<a name="objc-protobuf-tests-MessageContainingEnumCalledType-TypeEntry"></a>

### MessageContainingEnumCalledType.TypeEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [MessageContainingEnumCalledType](#objc-protobuf-tests-MessageContainingEnumCalledType) |  |  |






<a name="objc-protobuf-tests-MessageContainingMapCalledEntry"></a>

### MessageContainingMapCalledEntry
Previously, message cannot contain map field called &#34;entry&#34;.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| entry | [MessageContainingMapCalledEntry.EntryEntry](#objc-protobuf-tests-MessageContainingMapCalledEntry-EntryEntry) | repeated |  |






<a name="objc-protobuf-tests-MessageContainingMapCalledEntry-EntryEntry"></a>

### MessageContainingMapCalledEntry.EntryEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="objc-protobuf-tests-TestArenaMap"></a>

### TestArenaMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map_int32_int32 | [TestArenaMap.MapInt32Int32Entry](#objc-protobuf-tests-TestArenaMap-MapInt32Int32Entry) | repeated |  |
| map_int64_int64 | [TestArenaMap.MapInt64Int64Entry](#objc-protobuf-tests-TestArenaMap-MapInt64Int64Entry) | repeated |  |
| map_uint32_uint32 | [TestArenaMap.MapUint32Uint32Entry](#objc-protobuf-tests-TestArenaMap-MapUint32Uint32Entry) | repeated |  |
| map_uint64_uint64 | [TestArenaMap.MapUint64Uint64Entry](#objc-protobuf-tests-TestArenaMap-MapUint64Uint64Entry) | repeated |  |
| map_sint32_sint32 | [TestArenaMap.MapSint32Sint32Entry](#objc-protobuf-tests-TestArenaMap-MapSint32Sint32Entry) | repeated |  |
| map_sint64_sint64 | [TestArenaMap.MapSint64Sint64Entry](#objc-protobuf-tests-TestArenaMap-MapSint64Sint64Entry) | repeated |  |
| map_fixed32_fixed32 | [TestArenaMap.MapFixed32Fixed32Entry](#objc-protobuf-tests-TestArenaMap-MapFixed32Fixed32Entry) | repeated |  |
| map_fixed64_fixed64 | [TestArenaMap.MapFixed64Fixed64Entry](#objc-protobuf-tests-TestArenaMap-MapFixed64Fixed64Entry) | repeated |  |
| map_sfixed32_sfixed32 | [TestArenaMap.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-TestArenaMap-MapSfixed32Sfixed32Entry) | repeated |  |
| map_sfixed64_sfixed64 | [TestArenaMap.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-TestArenaMap-MapSfixed64Sfixed64Entry) | repeated |  |
| map_int32_float | [TestArenaMap.MapInt32FloatEntry](#objc-protobuf-tests-TestArenaMap-MapInt32FloatEntry) | repeated |  |
| map_int32_double | [TestArenaMap.MapInt32DoubleEntry](#objc-protobuf-tests-TestArenaMap-MapInt32DoubleEntry) | repeated |  |
| map_bool_bool | [TestArenaMap.MapBoolBoolEntry](#objc-protobuf-tests-TestArenaMap-MapBoolBoolEntry) | repeated |  |
| map_string_string | [TestArenaMap.MapStringStringEntry](#objc-protobuf-tests-TestArenaMap-MapStringStringEntry) | repeated |  |
| map_int32_bytes | [TestArenaMap.MapInt32BytesEntry](#objc-protobuf-tests-TestArenaMap-MapInt32BytesEntry) | repeated |  |
| map_int32_enum | [TestArenaMap.MapInt32EnumEntry](#objc-protobuf-tests-TestArenaMap-MapInt32EnumEntry) | repeated |  |
| map_int32_foreign_message | [TestArenaMap.MapInt32ForeignMessageEntry](#objc-protobuf-tests-TestArenaMap-MapInt32ForeignMessageEntry) | repeated |  |






<a name="objc-protobuf-tests-TestArenaMap-MapBoolBoolEntry"></a>

### TestArenaMap.MapBoolBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [bool](#bool) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapFixed32Fixed32Entry"></a>

### TestArenaMap.MapFixed32Fixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapFixed64Fixed64Entry"></a>

### TestArenaMap.MapFixed64Fixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt32BytesEntry"></a>

### TestArenaMap.MapInt32BytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt32DoubleEntry"></a>

### TestArenaMap.MapInt32DoubleEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [double](#double) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt32EnumEntry"></a>

### TestArenaMap.MapInt32EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [MapEnum](#objc-protobuf-tests-MapEnum) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt32FloatEntry"></a>

### TestArenaMap.MapInt32FloatEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [float](#float) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt32ForeignMessageEntry"></a>

### TestArenaMap.MapInt32ForeignMessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt32Int32Entry"></a>

### TestArenaMap.MapInt32Int32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapInt64Int64Entry"></a>

### TestArenaMap.MapInt64Int64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int64](#int64) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapSfixed32Sfixed32Entry"></a>

### TestArenaMap.MapSfixed32Sfixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapSfixed64Sfixed64Entry"></a>

### TestArenaMap.MapSfixed64Sfixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapSint32Sint32Entry"></a>

### TestArenaMap.MapSint32Sint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapSint64Sint64Entry"></a>

### TestArenaMap.MapSint64Sint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapStringStringEntry"></a>

### TestArenaMap.MapStringStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapUint32Uint32Entry"></a>

### TestArenaMap.MapUint32Uint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="objc-protobuf-tests-TestArenaMap-MapUint64Uint64Entry"></a>

### TestArenaMap.MapUint64Uint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="objc-protobuf-tests-TestMap"></a>

### TestMap
Tests maps.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map_int32_int32 | [TestMap.MapInt32Int32Entry](#objc-protobuf-tests-TestMap-MapInt32Int32Entry) | repeated |  |
| map_int64_int64 | [TestMap.MapInt64Int64Entry](#objc-protobuf-tests-TestMap-MapInt64Int64Entry) | repeated |  |
| map_uint32_uint32 | [TestMap.MapUint32Uint32Entry](#objc-protobuf-tests-TestMap-MapUint32Uint32Entry) | repeated |  |
| map_uint64_uint64 | [TestMap.MapUint64Uint64Entry](#objc-protobuf-tests-TestMap-MapUint64Uint64Entry) | repeated |  |
| map_sint32_sint32 | [TestMap.MapSint32Sint32Entry](#objc-protobuf-tests-TestMap-MapSint32Sint32Entry) | repeated |  |
| map_sint64_sint64 | [TestMap.MapSint64Sint64Entry](#objc-protobuf-tests-TestMap-MapSint64Sint64Entry) | repeated |  |
| map_fixed32_fixed32 | [TestMap.MapFixed32Fixed32Entry](#objc-protobuf-tests-TestMap-MapFixed32Fixed32Entry) | repeated |  |
| map_fixed64_fixed64 | [TestMap.MapFixed64Fixed64Entry](#objc-protobuf-tests-TestMap-MapFixed64Fixed64Entry) | repeated |  |
| map_sfixed32_sfixed32 | [TestMap.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-TestMap-MapSfixed32Sfixed32Entry) | repeated |  |
| map_sfixed64_sfixed64 | [TestMap.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-TestMap-MapSfixed64Sfixed64Entry) | repeated |  |
| map_int32_float | [TestMap.MapInt32FloatEntry](#objc-protobuf-tests-TestMap-MapInt32FloatEntry) | repeated |  |
| map_int32_double | [TestMap.MapInt32DoubleEntry](#objc-protobuf-tests-TestMap-MapInt32DoubleEntry) | repeated |  |
| map_bool_bool | [TestMap.MapBoolBoolEntry](#objc-protobuf-tests-TestMap-MapBoolBoolEntry) | repeated |  |
| map_string_string | [TestMap.MapStringStringEntry](#objc-protobuf-tests-TestMap-MapStringStringEntry) | repeated |  |
| map_int32_bytes | [TestMap.MapInt32BytesEntry](#objc-protobuf-tests-TestMap-MapInt32BytesEntry) | repeated |  |
| map_int32_enum | [TestMap.MapInt32EnumEntry](#objc-protobuf-tests-TestMap-MapInt32EnumEntry) | repeated |  |
| map_int32_foreign_message | [TestMap.MapInt32ForeignMessageEntry](#objc-protobuf-tests-TestMap-MapInt32ForeignMessageEntry) | repeated |  |
| map_string_foreign_message | [TestMap.MapStringForeignMessageEntry](#objc-protobuf-tests-TestMap-MapStringForeignMessageEntry) | repeated |  |
| map_int32_all_types | [TestMap.MapInt32AllTypesEntry](#objc-protobuf-tests-TestMap-MapInt32AllTypesEntry) | repeated |  |






<a name="objc-protobuf-tests-TestMap-MapBoolBoolEntry"></a>

### TestMap.MapBoolBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [bool](#bool) |  |  |






<a name="objc-protobuf-tests-TestMap-MapFixed32Fixed32Entry"></a>

### TestMap.MapFixed32Fixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="objc-protobuf-tests-TestMap-MapFixed64Fixed64Entry"></a>

### TestMap.MapFixed64Fixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32AllTypesEntry"></a>

### TestMap.MapInt32AllTypesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32BytesEntry"></a>

### TestMap.MapInt32BytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32DoubleEntry"></a>

### TestMap.MapInt32DoubleEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [double](#double) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32EnumEntry"></a>

### TestMap.MapInt32EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [MapEnum](#objc-protobuf-tests-MapEnum) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32FloatEntry"></a>

### TestMap.MapInt32FloatEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [float](#float) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32ForeignMessageEntry"></a>

### TestMap.MapInt32ForeignMessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt32Int32Entry"></a>

### TestMap.MapInt32Int32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="objc-protobuf-tests-TestMap-MapInt64Int64Entry"></a>

### TestMap.MapInt64Int64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int64](#int64) |  |  |






<a name="objc-protobuf-tests-TestMap-MapSfixed32Sfixed32Entry"></a>

### TestMap.MapSfixed32Sfixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="objc-protobuf-tests-TestMap-MapSfixed64Sfixed64Entry"></a>

### TestMap.MapSfixed64Sfixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="objc-protobuf-tests-TestMap-MapSint32Sint32Entry"></a>

### TestMap.MapSint32Sint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="objc-protobuf-tests-TestMap-MapSint64Sint64Entry"></a>

### TestMap.MapSint64Sint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="objc-protobuf-tests-TestMap-MapStringForeignMessageEntry"></a>

### TestMap.MapStringForeignMessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) |  |  |






<a name="objc-protobuf-tests-TestMap-MapStringStringEntry"></a>

### TestMap.MapStringStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="objc-protobuf-tests-TestMap-MapUint32Uint32Entry"></a>

### TestMap.MapUint32Uint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="objc-protobuf-tests-TestMap-MapUint64Uint64Entry"></a>

### TestMap.MapUint64Uint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="objc-protobuf-tests-TestMapSubmessage"></a>

### TestMapSubmessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| test_map | [TestMap](#objc-protobuf-tests-TestMap) |  |  |






<a name="objc-protobuf-tests-TestMessageMap"></a>

### TestMessageMap



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map_int32_message | [TestMessageMap.MapInt32MessageEntry](#objc-protobuf-tests-TestMessageMap-MapInt32MessageEntry) | repeated |  |






<a name="objc-protobuf-tests-TestMessageMap-MapInt32MessageEntry"></a>

### TestMessageMap.MapInt32MessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) |  |  |






<a name="objc-protobuf-tests-TestRecursiveMapMessage"></a>

### TestRecursiveMapMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [TestRecursiveMapMessage.AEntry](#objc-protobuf-tests-TestRecursiveMapMessage-AEntry) | repeated |  |






<a name="objc-protobuf-tests-TestRecursiveMapMessage-AEntry"></a>

### TestRecursiveMapMessage.AEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [TestRecursiveMapMessage](#objc-protobuf-tests-TestRecursiveMapMessage) |  |  |






<a name="objc-protobuf-tests-TestRequiredMessageMap"></a>

### TestRequiredMessageMap
Test embedded message with required fields


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map_field | [TestRequiredMessageMap.MapFieldEntry](#objc-protobuf-tests-TestRequiredMessageMap-MapFieldEntry) | repeated |  |






<a name="objc-protobuf-tests-TestRequiredMessageMap-MapFieldEntry"></a>

### TestRequiredMessageMap.MapFieldEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [TestRequired](#objc-protobuf-tests-TestRequired) |  |  |






<a name="objc-protobuf-tests-TestSameTypeMap"></a>

### TestSameTypeMap
Two map fields share the same entry default instance.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map1 | [TestSameTypeMap.Map1Entry](#objc-protobuf-tests-TestSameTypeMap-Map1Entry) | repeated |  |
| map2 | [TestSameTypeMap.Map2Entry](#objc-protobuf-tests-TestSameTypeMap-Map2Entry) | repeated |  |






<a name="objc-protobuf-tests-TestSameTypeMap-Map1Entry"></a>

### TestSameTypeMap.Map1Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="objc-protobuf-tests-TestSameTypeMap-Map2Entry"></a>

### TestSameTypeMap.Map2Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |





 


<a name="objc-protobuf-tests-MapEnum"></a>

### MapEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| MAP_ENUM_FOO | 0 |  |
| MAP_ENUM_BAR | 1 |  |
| MAP_ENUM_BAZ | 2 |  |



<a name="objc-protobuf-tests-MessageContainingEnumCalledType-Type"></a>

### MessageContainingEnumCalledType.Type


| Name | Number | Description |
| ---- | ------ | ----------- |
| TYPE_FOO | 0 |  |


 

 

 



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

