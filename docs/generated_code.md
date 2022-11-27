# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [ruby/compatibility_tests/v3.0.0/tests/generated_code.proto](#ruby_compatibility_tests_v3-0-0_tests_generated_code-proto)
    - [TestMessage](#a-b-c-TestMessage)
    - [TestMessage.MapBoolStringEntry](#a-b-c-TestMessage-MapBoolStringEntry)
    - [TestMessage.MapInt32StringEntry](#a-b-c-TestMessage-MapInt32StringEntry)
    - [TestMessage.MapInt64StringEntry](#a-b-c-TestMessage-MapInt64StringEntry)
    - [TestMessage.MapStringBoolEntry](#a-b-c-TestMessage-MapStringBoolEntry)
    - [TestMessage.MapStringEnumEntry](#a-b-c-TestMessage-MapStringEnumEntry)
    - [TestMessage.MapStringInt32Entry](#a-b-c-TestMessage-MapStringInt32Entry)
    - [TestMessage.MapStringMsgEntry](#a-b-c-TestMessage-MapStringMsgEntry)
    - [TestMessage.MapStringStringEntry](#a-b-c-TestMessage-MapStringStringEntry)
    - [TestMessage.MapUint32StringEntry](#a-b-c-TestMessage-MapUint32StringEntry)
    - [TestMessage.MapUint64StringEntry](#a-b-c-TestMessage-MapUint64StringEntry)
    - [TestMessage.NestedMessage](#a-b-c-TestMessage-NestedMessage)
  
    - [TestEnum](#a-b-c-TestEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="ruby_compatibility_tests_v3-0-0_tests_generated_code-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## ruby/compatibility_tests/v3.0.0/tests/generated_code.proto



<a name="a-b-c-TestMessage"></a>

### TestMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) |  |  |
| optional_int64 | [int64](#int64) |  |  |
| optional_uint32 | [uint32](#uint32) |  |  |
| optional_uint64 | [uint64](#uint64) |  |  |
| optional_bool | [bool](#bool) |  |  |
| optional_double | [double](#double) |  |  |
| optional_float | [float](#float) |  |  |
| optional_string | [string](#string) |  |  |
| optional_bytes | [bytes](#bytes) |  |  |
| optional_enum | [TestEnum](#a-b-c-TestEnum) |  |  |
| optional_msg | [TestMessage](#a-b-c-TestMessage) |  |  |
| repeated_int32 | [int32](#int32) | repeated |  |
| repeated_int64 | [int64](#int64) | repeated |  |
| repeated_uint32 | [uint32](#uint32) | repeated |  |
| repeated_uint64 | [uint64](#uint64) | repeated |  |
| repeated_bool | [bool](#bool) | repeated |  |
| repeated_double | [double](#double) | repeated |  |
| repeated_float | [float](#float) | repeated |  |
| repeated_string | [string](#string) | repeated |  |
| repeated_bytes | [bytes](#bytes) | repeated |  |
| repeated_enum | [TestEnum](#a-b-c-TestEnum) | repeated |  |
| repeated_msg | [TestMessage](#a-b-c-TestMessage) | repeated |  |
| oneof_int32 | [int32](#int32) |  |  |
| oneof_int64 | [int64](#int64) |  |  |
| oneof_uint32 | [uint32](#uint32) |  |  |
| oneof_uint64 | [uint64](#uint64) |  |  |
| oneof_bool | [bool](#bool) |  |  |
| oneof_double | [double](#double) |  |  |
| oneof_float | [float](#float) |  |  |
| oneof_string | [string](#string) |  |  |
| oneof_bytes | [bytes](#bytes) |  |  |
| oneof_enum | [TestEnum](#a-b-c-TestEnum) |  |  |
| oneof_msg | [TestMessage](#a-b-c-TestMessage) |  |  |
| map_int32_string | [TestMessage.MapInt32StringEntry](#a-b-c-TestMessage-MapInt32StringEntry) | repeated |  |
| map_int64_string | [TestMessage.MapInt64StringEntry](#a-b-c-TestMessage-MapInt64StringEntry) | repeated |  |
| map_uint32_string | [TestMessage.MapUint32StringEntry](#a-b-c-TestMessage-MapUint32StringEntry) | repeated |  |
| map_uint64_string | [TestMessage.MapUint64StringEntry](#a-b-c-TestMessage-MapUint64StringEntry) | repeated |  |
| map_bool_string | [TestMessage.MapBoolStringEntry](#a-b-c-TestMessage-MapBoolStringEntry) | repeated |  |
| map_string_string | [TestMessage.MapStringStringEntry](#a-b-c-TestMessage-MapStringStringEntry) | repeated |  |
| map_string_msg | [TestMessage.MapStringMsgEntry](#a-b-c-TestMessage-MapStringMsgEntry) | repeated |  |
| map_string_enum | [TestMessage.MapStringEnumEntry](#a-b-c-TestMessage-MapStringEnumEntry) | repeated |  |
| map_string_int32 | [TestMessage.MapStringInt32Entry](#a-b-c-TestMessage-MapStringInt32Entry) | repeated |  |
| map_string_bool | [TestMessage.MapStringBoolEntry](#a-b-c-TestMessage-MapStringBoolEntry) | repeated |  |
| nested_message | [TestMessage.NestedMessage](#a-b-c-TestMessage-NestedMessage) |  |  |






<a name="a-b-c-TestMessage-MapBoolStringEntry"></a>

### TestMessage.MapBoolStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [string](#string) |  |  |






<a name="a-b-c-TestMessage-MapInt32StringEntry"></a>

### TestMessage.MapInt32StringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [string](#string) |  |  |






<a name="a-b-c-TestMessage-MapInt64StringEntry"></a>

### TestMessage.MapInt64StringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [string](#string) |  |  |






<a name="a-b-c-TestMessage-MapStringBoolEntry"></a>

### TestMessage.MapStringBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bool](#bool) |  |  |






<a name="a-b-c-TestMessage-MapStringEnumEntry"></a>

### TestMessage.MapStringEnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [TestEnum](#a-b-c-TestEnum) |  |  |






<a name="a-b-c-TestMessage-MapStringInt32Entry"></a>

### TestMessage.MapStringInt32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="a-b-c-TestMessage-MapStringMsgEntry"></a>

### TestMessage.MapStringMsgEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [TestMessage](#a-b-c-TestMessage) |  |  |






<a name="a-b-c-TestMessage-MapStringStringEntry"></a>

### TestMessage.MapStringStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="a-b-c-TestMessage-MapUint32StringEntry"></a>

### TestMessage.MapUint32StringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [string](#string) |  |  |






<a name="a-b-c-TestMessage-MapUint64StringEntry"></a>

### TestMessage.MapUint64StringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [string](#string) |  |  |






<a name="a-b-c-TestMessage-NestedMessage"></a>

### TestMessage.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [int32](#int32) |  |  |





 


<a name="a-b-c-TestEnum"></a>

### TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| Default | 0 |  |
| A | 1 |  |
| B | 2 |  |
| C | 3 |  |


 

 

 



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

