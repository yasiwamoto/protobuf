# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_runtime_proto3.proto](#objectivec_Tests_unittest_runtime_proto3-proto)
    - [Message3](#objc-protobuf-tests-Message3)
    - [Message3.MapBoolBoolEntry](#objc-protobuf-tests-Message3-MapBoolBoolEntry)
    - [Message3.MapFixed32Fixed32Entry](#objc-protobuf-tests-Message3-MapFixed32Fixed32Entry)
    - [Message3.MapFixed64Fixed64Entry](#objc-protobuf-tests-Message3-MapFixed64Fixed64Entry)
    - [Message3.MapInt32BytesEntry](#objc-protobuf-tests-Message3-MapInt32BytesEntry)
    - [Message3.MapInt32DoubleEntry](#objc-protobuf-tests-Message3-MapInt32DoubleEntry)
    - [Message3.MapInt32EnumEntry](#objc-protobuf-tests-Message3-MapInt32EnumEntry)
    - [Message3.MapInt32FloatEntry](#objc-protobuf-tests-Message3-MapInt32FloatEntry)
    - [Message3.MapInt32Int32Entry](#objc-protobuf-tests-Message3-MapInt32Int32Entry)
    - [Message3.MapInt32MessageEntry](#objc-protobuf-tests-Message3-MapInt32MessageEntry)
    - [Message3.MapInt64Int64Entry](#objc-protobuf-tests-Message3-MapInt64Int64Entry)
    - [Message3.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-Message3-MapSfixed32Sfixed32Entry)
    - [Message3.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-Message3-MapSfixed64Sfixed64Entry)
    - [Message3.MapSint32Sint32Entry](#objc-protobuf-tests-Message3-MapSint32Sint32Entry)
    - [Message3.MapSint64Sint64Entry](#objc-protobuf-tests-Message3-MapSint64Sint64Entry)
    - [Message3.MapStringBytesEntry](#objc-protobuf-tests-Message3-MapStringBytesEntry)
    - [Message3.MapStringMessageEntry](#objc-protobuf-tests-Message3-MapStringMessageEntry)
    - [Message3.MapStringStringEntry](#objc-protobuf-tests-Message3-MapStringStringEntry)
    - [Message3.MapUint32Uint32Entry](#objc-protobuf-tests-Message3-MapUint32Uint32Entry)
    - [Message3.MapUint64Uint64Entry](#objc-protobuf-tests-Message3-MapUint64Uint64Entry)
    - [Message3Optional](#objc-protobuf-tests-Message3Optional)
  
    - [Message3.Enum](#objc-protobuf-tests-Message3-Enum)
    - [Message3Optional.Enum](#objc-protobuf-tests-Message3Optional-Enum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_runtime_proto3-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_runtime_proto3.proto



<a name="objc-protobuf-tests-Message3"></a>

### Message3



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
| optional_message | [Message3](#objc-protobuf-tests-Message3) |  | No &#39;group&#39; in proto3. |
| optional_enum | [Message3.Enum](#objc-protobuf-tests-Message3-Enum) |  |  |
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
| repeated_message | [Message3](#objc-protobuf-tests-Message3) | repeated | No &#39;group&#39; in proto3. |
| repeated_enum | [Message3.Enum](#objc-protobuf-tests-Message3-Enum) | repeated |  |
| oneof_int32 | [int32](#int32) |  |  |
| oneof_int64 | [int64](#int64) |  |  |
| oneof_uint32 | [uint32](#uint32) |  |  |
| oneof_uint64 | [uint64](#uint64) |  |  |
| oneof_sint32 | [sint32](#sint32) |  |  |
| oneof_sint64 | [sint64](#sint64) |  |  |
| oneof_fixed32 | [fixed32](#fixed32) |  |  |
| oneof_fixed64 | [fixed64](#fixed64) |  |  |
| oneof_sfixed32 | [sfixed32](#sfixed32) |  |  |
| oneof_sfixed64 | [sfixed64](#sfixed64) |  |  |
| oneof_float | [float](#float) |  |  |
| oneof_double | [double](#double) |  |  |
| oneof_bool | [bool](#bool) |  |  |
| oneof_string | [string](#string) |  |  |
| oneof_bytes | [bytes](#bytes) |  |  |
| oneof_message | [Message3](#objc-protobuf-tests-Message3) |  | No &#39;group&#39; in proto3. |
| oneof_enum | [Message3.Enum](#objc-protobuf-tests-Message3-Enum) |  |  |
| map_int32_int32 | [Message3.MapInt32Int32Entry](#objc-protobuf-tests-Message3-MapInt32Int32Entry) | repeated | Some token map cases, too many combinations to list them all. |
| map_int64_int64 | [Message3.MapInt64Int64Entry](#objc-protobuf-tests-Message3-MapInt64Int64Entry) | repeated |  |
| map_uint32_uint32 | [Message3.MapUint32Uint32Entry](#objc-protobuf-tests-Message3-MapUint32Uint32Entry) | repeated |  |
| map_uint64_uint64 | [Message3.MapUint64Uint64Entry](#objc-protobuf-tests-Message3-MapUint64Uint64Entry) | repeated |  |
| map_sint32_sint32 | [Message3.MapSint32Sint32Entry](#objc-protobuf-tests-Message3-MapSint32Sint32Entry) | repeated |  |
| map_sint64_sint64 | [Message3.MapSint64Sint64Entry](#objc-protobuf-tests-Message3-MapSint64Sint64Entry) | repeated |  |
| map_fixed32_fixed32 | [Message3.MapFixed32Fixed32Entry](#objc-protobuf-tests-Message3-MapFixed32Fixed32Entry) | repeated |  |
| map_fixed64_fixed64 | [Message3.MapFixed64Fixed64Entry](#objc-protobuf-tests-Message3-MapFixed64Fixed64Entry) | repeated |  |
| map_sfixed32_sfixed32 | [Message3.MapSfixed32Sfixed32Entry](#objc-protobuf-tests-Message3-MapSfixed32Sfixed32Entry) | repeated |  |
| map_sfixed64_sfixed64 | [Message3.MapSfixed64Sfixed64Entry](#objc-protobuf-tests-Message3-MapSfixed64Sfixed64Entry) | repeated |  |
| map_int32_float | [Message3.MapInt32FloatEntry](#objc-protobuf-tests-Message3-MapInt32FloatEntry) | repeated |  |
| map_int32_double | [Message3.MapInt32DoubleEntry](#objc-protobuf-tests-Message3-MapInt32DoubleEntry) | repeated |  |
| map_bool_bool | [Message3.MapBoolBoolEntry](#objc-protobuf-tests-Message3-MapBoolBoolEntry) | repeated |  |
| map_string_string | [Message3.MapStringStringEntry](#objc-protobuf-tests-Message3-MapStringStringEntry) | repeated |  |
| map_string_bytes | [Message3.MapStringBytesEntry](#objc-protobuf-tests-Message3-MapStringBytesEntry) | repeated |  |
| map_string_message | [Message3.MapStringMessageEntry](#objc-protobuf-tests-Message3-MapStringMessageEntry) | repeated |  |
| map_int32_bytes | [Message3.MapInt32BytesEntry](#objc-protobuf-tests-Message3-MapInt32BytesEntry) | repeated |  |
| map_int32_enum | [Message3.MapInt32EnumEntry](#objc-protobuf-tests-Message3-MapInt32EnumEntry) | repeated |  |
| map_int32_message | [Message3.MapInt32MessageEntry](#objc-protobuf-tests-Message3-MapInt32MessageEntry) | repeated |  |






<a name="objc-protobuf-tests-Message3-MapBoolBoolEntry"></a>

### Message3.MapBoolBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [bool](#bool) |  |  |






<a name="objc-protobuf-tests-Message3-MapFixed32Fixed32Entry"></a>

### Message3.MapFixed32Fixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="objc-protobuf-tests-Message3-MapFixed64Fixed64Entry"></a>

### Message3.MapFixed64Fixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt32BytesEntry"></a>

### Message3.MapInt32BytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt32DoubleEntry"></a>

### Message3.MapInt32DoubleEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [double](#double) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt32EnumEntry"></a>

### Message3.MapInt32EnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [Message3.Enum](#objc-protobuf-tests-Message3-Enum) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt32FloatEntry"></a>

### Message3.MapInt32FloatEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [float](#float) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt32Int32Entry"></a>

### Message3.MapInt32Int32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt32MessageEntry"></a>

### Message3.MapInt32MessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [Message3](#objc-protobuf-tests-Message3) |  |  |






<a name="objc-protobuf-tests-Message3-MapInt64Int64Entry"></a>

### Message3.MapInt64Int64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int64](#int64) |  |  |






<a name="objc-protobuf-tests-Message3-MapSfixed32Sfixed32Entry"></a>

### Message3.MapSfixed32Sfixed32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="objc-protobuf-tests-Message3-MapSfixed64Sfixed64Entry"></a>

### Message3.MapSfixed64Sfixed64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="objc-protobuf-tests-Message3-MapSint32Sint32Entry"></a>

### Message3.MapSint32Sint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="objc-protobuf-tests-Message3-MapSint64Sint64Entry"></a>

### Message3.MapSint64Sint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="objc-protobuf-tests-Message3-MapStringBytesEntry"></a>

### Message3.MapStringBytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="objc-protobuf-tests-Message3-MapStringMessageEntry"></a>

### Message3.MapStringMessageEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [Message3](#objc-protobuf-tests-Message3) |  |  |






<a name="objc-protobuf-tests-Message3-MapStringStringEntry"></a>

### Message3.MapStringStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="objc-protobuf-tests-Message3-MapUint32Uint32Entry"></a>

### Message3.MapUint32Uint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="objc-protobuf-tests-Message3-MapUint64Uint64Entry"></a>

### Message3.MapUint64Uint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="objc-protobuf-tests-Message3Optional"></a>

### Message3Optional



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
| optional_message | [Message3](#objc-protobuf-tests-Message3) | optional | No &#39;group&#39; in proto3. |
| optional_enum | [Message3Optional.Enum](#objc-protobuf-tests-Message3Optional-Enum) | optional |  |





 


<a name="objc-protobuf-tests-Message3-Enum"></a>

### Message3.Enum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |
| BAR | 1 |  |
| BAZ | 2 |  |
| EXTRA_3 | 30 |  |



<a name="objc-protobuf-tests-Message3Optional-Enum"></a>

### Message3Optional.Enum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |
| BAR | 1 |  |
| BAZ | 2 |  |
| EXTRA_3 | 30 |  |


 

 

 



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

