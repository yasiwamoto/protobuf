# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_runtime_proto2.proto](#objectivec_Tests_unittest_runtime_proto2-proto)
    - [Message2](#objc-protobuf-tests-Message2)
    - [Message2.MapBoolBoolEntry](#objc-protobuf-tests-Message2-MapBoolBoolEntry)
    - [Message2.MapFixed32Fixed32Entry](#objc-protobuf-tests-Message2-MapFixed32Fixed32Entry)
    - [Message2.MapFixed64Fixed64Entry](#objc-protobuf-tests-Message2-MapFixed64Fixed64Entry)
    - [Message2.MapInt32BytesEntry](#objc-protobuf-tests-Message2-MapInt32BytesEntry)
    - [Message2.MapInt32DoubleEntry](#objc-protobuf-tests-Message2-MapInt32DoubleEntry)
    - [Message2.MapInt32EnumEntry](#objc-protobuf-tests-Message2-MapInt32EnumEntry)
    - [Message2.MapInt32FloatEntry](#objc-protobuf-tests-Message2-MapInt32FloatEntry)
    - [Message2.MapInt32Int32Entry](#objc-protobuf-tests-Message2-MapInt32Int32Entry)
    - [Message2.MapInt32MessageEntry](#objc-protobuf-tests-Message2-MapInt32MessageEntry)
    - [Message2.MapInt64Int64Entry](#objc-protobuf-tests-Message2-MapInt64Int64Entry)
    - [Message2.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-Message2-MapSfixed32Sfixed32Entry)
    - [Message2.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-Message2-MapSfixed64Sfixed64Entry)
    - [Message2.MapSint32Sint32Entry](#objc-protobuf-tests-Message2-MapSint32Sint32Entry)
    - [Message2.MapSint64Sint64Entry](#objc-protobuf-tests-Message2-MapSint64Sint64Entry)
    - [Message2.MapStringBytesEntry](#objc-protobuf-tests-Message2-MapStringBytesEntry)
    - [Message2.MapStringMessageEntry](#objc-protobuf-tests-Message2-MapStringMessageEntry)
    - [Message2.MapStringStringEntry](#objc-protobuf-tests-Message2-MapStringStringEntry)
    - [Message2.MapUint32Uint32Entry](#objc-protobuf-tests-Message2-MapUint32Uint32Entry)
    - [Message2.MapUint64Uint64Entry](#objc-protobuf-tests-Message2-MapUint64Uint64Entry)
    - [Message2.OneofGroup](#objc-protobuf-tests-Message2-OneofGroup)
    - [Message2.OptionalGroup](#objc-protobuf-tests-Message2-OptionalGroup)
    - [Message2.RepeatedGroup](#objc-protobuf-tests-Message2-RepeatedGroup)
  
    - [Message2.Enum](#objc-protobuf-tests-Message2-Enum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_runtime_proto2-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_runtime_proto2.proto



<a name="objc-protobuf-tests-Message2"></a>

### Message2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) | optional |  |
| optional_int64 | [int64](#int64) | optional |  |
| optional_uint32 | [uint32](#uint32) | optional |  |
| optional_uint64 | [uint64](#uint64) | optional |  |
| optional_sint32 | [sint32](#sint32) | optional |  |
| optional_sint64 | [sint64](#sint64) | optional |  |
| optional_fixed32 | [fixed32](#fixed32) | optional |  |
| optional_fixed64 | [fixed64](#fixed64) | optional |  |
| optional_sfixed32 | [sfixed32](#sfixed32) | optional |  |
| optional_sfixed64 | [sfixed64](#sfixed64) | optional |  |
| optional_float | [float](#float) | optional |  |
| optional_double | [double](#double) | optional |  |
| optional_bool | [bool](#bool) | optional |  |
| optional_string | [string](#string) | optional |  |
| optional_bytes | [bytes](#bytes) | optional |  |
| optionalgroup | [Message2.OptionalGroup](#objc-protobuf-tests-Message2-OptionalGroup) | optional |  |
| optional_message | [Message2](#objc-protobuf-tests-Message2) | optional |  |
| optional_enum | [Message2.Enum](#objc-protobuf-tests-Message2-Enum) | optional |  |
| repeated_int32 | [int32](#int32) | repeated |  |
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
| repeatedgroup | [Message2.RepeatedGroup](#objc-protobuf-tests-Message2-RepeatedGroup) | repeated |  |
| repeated_message | [Message2](#objc-protobuf-tests-Message2) | repeated |  |
| repeated_enum | [Message2.Enum](#objc-protobuf-tests-Message2-Enum) | repeated |  |
| oneof_int32 | [int32](#int32) | optional |  Default: 100 |
| oneof_int64 | [int64](#int64) | optional |  Default: 101 |
| oneof_uint32 | [uint32](#uint32) | optional |  Default: 102 |
| oneof_uint64 | [uint64](#uint64) | optional |  Default: 103 |
| oneof_sint32 | [sint32](#sint32) | optional |  Default: 104 |
| oneof_sint64 | [sint64](#sint64) | optional |  Default: 105 |
| oneof_fixed32 | [fixed32](#fixed32) | optional |  Default: 106 |
| oneof_fixed64 | [fixed64](#fixed64) | optional |  Default: 107 |
| oneof_sfixed32 | [sfixed32](#sfixed32) | optional |  Default: 108 |
| oneof_sfixed64 | [sfixed64](#sfixed64) | optional |  Default: 109 |
| oneof_float | [float](#float) | optional |  Default: 110 |
| oneof_double | [double](#double) | optional |  Default: 111 |
| oneof_bool | [bool](#bool) | optional |  Default: true |
| oneof_string | [string](#string) | optional |  Default: string |
| oneof_bytes | [bytes](#bytes) | optional |  Default: data |
| oneofgroup | [Message2.OneofGroup](#objc-protobuf-tests-Message2-OneofGroup) | optional |  |
| oneof_message | [Message2](#objc-protobuf-tests-Message2) | optional |  |
| oneof_enum | [Message2.Enum](#objc-protobuf-tests-Message2-Enum) | optional |  Default: BAZ |
| map_int32_int32 | [Message2.MapInt32Int32Entry](#objc-protobuf-tests-Message2-MapInt32Int32Entry) | repeated | Some token map cases, too many combinations to list them all. |
| map_int64_int64 | [Message2.MapInt64Int64Entry](#objc-protobuf-tests-Message2-MapInt64Int64Entry) | repeated |  |
| map_uint32_uint32 | [Message2.MapUint32Uint32Entry](#objc-protobuf-tests-Message2-MapUint32Uint32Entry) | repeated |  |
| map_uint64_uint64 | [Message2.MapUint64Uint64Entry](#objc-protobuf-tests-Message2-MapUint64Uint64Entry) | repeated |  |
| map_sint32_sint32 | [Message2.MapSint32Sint32Entry](#objc-protobuf-tests-Message2-MapSint32Sint32Entry) | repeated |  |
| map_sint64_sint64 | [Message2.MapSint64Sint64Entry](#objc-protobuf-tests-Message2-MapSint64Sint64Entry) | repeated |  |
| map_fixed32_fixed32 | [Message2.MapFixed32Fixed32Entry](#objc-protobuf-tests-Message2-MapFixed32Fixed32Entry) | repeated |  |
| map_fixed64_fixed64 | [Message2.MapFixed64Fixed64Entry](#objc-protobuf-tests-Message2-MapFixed64Fixed64Entry) | repeated |  |
| map_sfixed32_sfixed32 | [Message2.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-Message2-MapSfixed32Sfixed32Entry) | repeated |  |
| map_sfixed64_sfixed64 | [Message2.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-Message2-MapSfixed64Sfixed64Entry) | repeated |  |
| map_int32_float | [Message2.MapInt32FloatEntry](#objc-protobuf-tests-Message2-MapInt32FloatEntry) | repeated |  |
| map_int32_double | [Message2.MapInt32DoubleEntry](#objc-protobuf-tests-Message2-MapInt32DoubleEntry) | repeated |  |
| map_bool_bool | [Message2.MapBoolBoolEntry](#objc-protobuf-tests-Message2-MapBoolBoolEntry) | repeated |  |
| map_string_string | [Message2.MapStringStringEntry](#objc-protobuf-tests-Message2-MapStringStringEntry) | repeated |  |
| map_string_bytes | [Message2.MapStringBytesEntry](#objc-protobuf-tests-Message2-MapStringBytesEntry) | repeated |  |
| map_string_message | [Message2.MapStringMessageEntry](#objc-protobuf-tests-Message2-MapStringMessageEntry) | repeated |  |
| map_int32_bytes | [Message2.MapInt32BytesEntry](#objc-protobuf-tests-Message2-MapInt32BytesEntry) | repeated |  |
| map_int32_enum | [Message2.MapInt32EnumEntry](#objc-protobuf-tests-Message2-MapInt32EnumEntry) | repeated |  |
| map_int32_message | [Message2.MapInt32MessageEntry](#objc-protobuf-tests-Message2-MapInt32MessageEntry) | repeated |  |






<a name="objc-protobuf-tests-Message2-MapBoolBoolEntry"></a>

### Message2.MapBoolBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="objc-protobuf-tests-Message2-MapFixed32Fixed32Entry"></a>

### Message2.MapFixed32Fixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="objc-protobuf-tests-Message2-MapFixed64Fixed64Entry"></a>

### Message2.MapFixed64Fixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt32BytesEntry"></a>

### Message2.MapInt32BytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt32DoubleEntry"></a>

### Message2.MapInt32DoubleEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [double](#double) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt32EnumEntry"></a>

### Message2.MapInt32EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Message2.Enum](#objc-protobuf-tests-Message2-Enum) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt32FloatEntry"></a>

### Message2.MapInt32FloatEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [float](#float) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt32Int32Entry"></a>

### Message2.MapInt32Int32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt32MessageEntry"></a>

### Message2.MapInt32MessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Message2](#objc-protobuf-tests-Message2) | optional |  |






<a name="objc-protobuf-tests-Message2-MapInt64Int64Entry"></a>

### Message2.MapInt64Int64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="objc-protobuf-tests-Message2-MapSfixed32Sfixed32Entry"></a>

### Message2.MapSfixed32Sfixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="objc-protobuf-tests-Message2-MapSfixed64Sfixed64Entry"></a>

### Message2.MapSfixed64Sfixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="objc-protobuf-tests-Message2-MapSint32Sint32Entry"></a>

### Message2.MapSint32Sint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="objc-protobuf-tests-Message2-MapSint64Sint64Entry"></a>

### Message2.MapSint64Sint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="objc-protobuf-tests-Message2-MapStringBytesEntry"></a>

### Message2.MapStringBytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="objc-protobuf-tests-Message2-MapStringMessageEntry"></a>

### Message2.MapStringMessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [Message2](#objc-protobuf-tests-Message2) | optional |  |






<a name="objc-protobuf-tests-Message2-MapStringStringEntry"></a>

### Message2.MapStringStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="objc-protobuf-tests-Message2-MapUint32Uint32Entry"></a>

### Message2.MapUint32Uint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="objc-protobuf-tests-Message2-MapUint64Uint64Entry"></a>

### Message2.MapUint64Uint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="objc-protobuf-tests-Message2-OneofGroup"></a>

### Message2.OneofGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| b | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-Message2-OptionalGroup"></a>

### Message2.OptionalGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-Message2-RepeatedGroup"></a>

### Message2.RepeatedGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |





 


<a name="objc-protobuf-tests-Message2-Enum"></a>

### Message2.Enum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |
| BAR | 1 |  |
| BAZ | 2 |  |
| EXTRA_2 | 20 |  |


 

 

 



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

