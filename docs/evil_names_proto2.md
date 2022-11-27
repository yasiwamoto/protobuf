# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/kotlin/src/test/proto/com/google/protobuf/evil_names_proto2.proto](#java_kotlin_src_test_proto_com_google_protobuf_evil_names_proto2-proto)
    - [EvilNamesProto2](#protobuf-kotlin-generator-EvilNamesProto2)
    - [EvilNamesProto2.ALLCAPSMAPEntry](#protobuf-kotlin-generator-EvilNamesProto2-ALLCAPSMAPEntry)
    - [HardKeywordsAllTypesProto2](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2)
    - [HardKeywordsAllTypesProto2.ContinueEntry](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-ContinueEntry)
    - [HardKeywordsAllTypesProto2.NestedMessage](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedMessage)
    - [Interface](#protobuf-kotlin-generator-Interface)
  
    - [HardKeywordsAllTypesProto2.NestedEnum](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_kotlin_src_test_proto_com_google_protobuf_evil_names_proto2-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/kotlin/src/test/proto/com/google/protobuf/evil_names_proto2.proto
LINT: LEGACY_NAMES


<a name="protobuf-kotlin-generator-EvilNamesProto2"></a>

### EvilNamesProto2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| initialized | [bool](#bool) | optional |  |
| has_foo | [bool](#bool) | optional |  |
| Bar | [string](#string) | optional |  |
| is_initialized | [bool](#bool) | optional |  |
| fooBar | [string](#string) | optional |  |
| ALL_CAPS | [string](#string) | repeated |  |
| ALL_CAPS_MAP | [EvilNamesProto2.ALLCAPSMAPEntry](#protobuf-kotlin-generator-EvilNamesProto2-ALLCAPSMAPEntry) | repeated |  |
| has_underbar_preceding_numeric_1foo | [bool](#bool) | optional |  |
| has_underbar_preceding_numeric_42bar | [bool](#bool) | optional |  |
| has_underbar_preceding_numeric_123foo42bar_baz | [bool](#bool) | optional |  |
| extension | [string](#string) | repeated |  |
| class | [int32](#int32) | repeated |  |
| int | [double](#double) | optional |  |
| long | [bool](#bool) | optional |  |
| boolean | [int64](#int64) | optional |  |
| sealed | [string](#string) | optional |  |
| interface | [float](#float) | optional |  |
| object | [string](#string) | optional |  |
| cached_size | [string](#string) | optional |  |
| serialized_size | [bool](#bool) | optional |  |
| by | [string](#string) | optional |  |






<a name="protobuf-kotlin-generator-EvilNamesProto2-ALLCAPSMAPEntry"></a>

### EvilNamesProto2.ALLCAPSMAPEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto2"></a>

### HardKeywordsAllTypesProto2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| as | [int32](#int32) | optional |  |
| break | [HardKeywordsAllTypesProto2.NestedEnum](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedEnum) | optional |  |
| continue | [HardKeywordsAllTypesProto2.ContinueEntry](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-ContinueEntry) | repeated |  |
| do | [HardKeywordsAllTypesProto2.NestedMessage](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedMessage) | optional |  |
| else | [int32](#int32) | repeated |  |
| for | [string](#string) | repeated |  |
| fun | [HardKeywordsAllTypesProto2.NestedEnum](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedEnum) | repeated |  |
| if | [HardKeywordsAllTypesProto2.NestedMessage](#protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedMessage) | repeated |  |






<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto2-ContinueEntry"></a>

### HardKeywordsAllTypesProto2.ContinueEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedMessage"></a>

### HardKeywordsAllTypesProto2.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| while | [int32](#int32) | optional |  |






<a name="protobuf-kotlin-generator-Interface"></a>

### Interface






 


<a name="protobuf-kotlin-generator-HardKeywordsAllTypesProto2-NestedEnum"></a>

### HardKeywordsAllTypesProto2.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
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

