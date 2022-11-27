# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/kotlin/src/test/proto/com/google/protobuf/evil_names_proto3.proto](#java_kotlin_src_test_proto_com_google_protobuf_evil_names_proto3-proto)
    - [Class](#protobuf-kotlin-generator-Class)
    - [EvilNamesProto3](#protobuf-kotlin-generator-EvilNamesProto3)
    - [EvilNamesProto3.ALLCAPSMAPEntry](#protobuf-kotlin-generator-EvilNamesProto3-ALLCAPSMAPEntry)
    - [EvilNamesProto3.KEntry](#protobuf-kotlin-generator-EvilNamesProto3-KEntry)
    - [EvilNamesProto3.KeyEntry](#protobuf-kotlin-generator-EvilNamesProto3-KeyEntry)
    - [EvilNamesProto3.MapEntry](#protobuf-kotlin-generator-EvilNamesProto3-MapEntry)
    - [EvilNamesProto3.PairsEntry](#protobuf-kotlin-generator-EvilNamesProto3-PairsEntry)
    - [EvilNamesProto3.VEntry](#protobuf-kotlin-generator-EvilNamesProto3-VEntry)
    - [HardKeywordsAllTypesProto3](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3)
    - [HardKeywordsAllTypesProto3.ContinueEntry](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-ContinueEntry)
    - [HardKeywordsAllTypesProto3.NestedMessage](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedMessage)
  
    - [HardKeywordsAllTypesProto3.NestedEnum](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_kotlin_src_test_proto_com_google_protobuf_evil_names_proto3-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/kotlin/src/test/proto/com/google/protobuf/evil_names_proto3.proto
LINT: LEGACY_NAMES


<a name="protobuf-kotlin-generator-Class"></a>

### Class







<a name="protobuf-kotlin-generator-EvilNamesProto3"></a>

### EvilNamesProto3



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| initialized | [bool](#bool) |  |  |
| has_foo | [bool](#bool) |  |  |
| Bar | [string](#string) |  |  |
| is_initialized | [bool](#bool) |  |  |
| fooBar | [string](#string) |  |  |
| ALL_CAPS | [string](#string) | repeated |  |
| ALL_CAPS_MAP | [EvilNamesProto3.ALLCAPSMAPEntry](#protobuf-kotlin-generator-EvilNamesProto3-ALLCAPSMAPEntry) | repeated |  |
| has_underbar_preceding_numeric_1foo | [bool](#bool) |  |  |
| has_underbar_preceding_numeric_42bar | [bool](#bool) |  |  |
| has_underbar_preceding_numeric_123foo42bar_baz | [bool](#bool) |  |  |
| extension | [string](#string) | repeated |  |
| class | [string](#string) |  |  |
| int | [double](#double) |  |  |
| long | [bool](#bool) |  |  |
| boolean | [int64](#int64) |  |  |
| sealed | [string](#string) |  |  |
| interface | [float](#float) |  |  |
| in | [int32](#int32) |  |  |
| object | [string](#string) |  |  |
| cached_size | [string](#string) |  |  |
| serialized_size | [bool](#bool) |  |  |
| value | [string](#string) |  |  |
| index | [int64](#int64) |  |  |
| values | [string](#string) | repeated |  |
| new_values | [string](#string) | repeated |  |
| builder | [bool](#bool) |  |  |
| k | [EvilNamesProto3.KEntry](#protobuf-kotlin-generator-EvilNamesProto3-KEntry) | repeated |  |
| v | [EvilNamesProto3.VEntry](#protobuf-kotlin-generator-EvilNamesProto3-VEntry) | repeated |  |
| key | [EvilNamesProto3.KeyEntry](#protobuf-kotlin-generator-EvilNamesProto3-KeyEntry) | repeated |  |
| map | [EvilNamesProto3.MapEntry](#protobuf-kotlin-generator-EvilNamesProto3-MapEntry) | repeated |  |
| pairs | [EvilNamesProto3.PairsEntry](#protobuf-kotlin-generator-EvilNamesProto3-PairsEntry) | repeated |  |
| _leading_underscore | [string](#string) |  |  |
| option | [int32](#int32) |  |  |






<a name="protobuf-kotlin-generator-EvilNamesProto3-ALLCAPSMAPEntry"></a>

### EvilNamesProto3.ALLCAPSMAPEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-kotlin-generator-EvilNamesProto3-KEntry"></a>

### EvilNamesProto3.KEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-kotlin-generator-EvilNamesProto3-KeyEntry"></a>

### EvilNamesProto3.KeyEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-kotlin-generator-EvilNamesProto3-MapEntry"></a>

### EvilNamesProto3.MapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-kotlin-generator-EvilNamesProto3-PairsEntry"></a>

### EvilNamesProto3.PairsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-kotlin-generator-EvilNamesProto3-VEntry"></a>

### EvilNamesProto3.VEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto3"></a>

### HardKeywordsAllTypesProto3



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| as | [int32](#int32) | optional |  |
| in | [string](#string) | optional |  |
| break | [HardKeywordsAllTypesProto3.NestedEnum](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedEnum) | optional |  |
| continue | [HardKeywordsAllTypesProto3.ContinueEntry](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-ContinueEntry) | repeated |  |
| do | [HardKeywordsAllTypesProto3.NestedMessage](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedMessage) | optional |  |
| else | [int32](#int32) | repeated |  |
| for | [string](#string) | repeated |  |
| fun | [HardKeywordsAllTypesProto3.NestedEnum](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedEnum) | repeated |  |
| if | [HardKeywordsAllTypesProto3.NestedMessage](#protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedMessage) | repeated |  |






<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto3-ContinueEntry"></a>

### HardKeywordsAllTypesProto3.ContinueEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedMessage"></a>

### HardKeywordsAllTypesProto3.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| while | [int32](#int32) | optional |  |





 


<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto3-NestedEnum"></a>

### HardKeywordsAllTypesProto3.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| FOO | 1 |  |
| BAR | 2 |  |


 

 

 



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

