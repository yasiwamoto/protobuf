# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [ruby/tests/basic_test.proto](#ruby_tests_basic_test-proto)
    - [Bar](#basic_test-Bar)
    - [Baz](#basic_test-Baz)
    - [Enumer](#basic_test-Enumer)
    - [Foo](#basic_test-Foo)
    - [HelloRequest](#basic_test-HelloRequest)
    - [Inner](#basic_test-Inner)
    - [MapMessage](#basic_test-MapMessage)
    - [MapMessage.MapStringEnumEntry](#basic_test-MapMessage-MapStringEnumEntry)
    - [MapMessage.MapStringInt32Entry](#basic_test-MapMessage-MapStringInt32Entry)
    - [MapMessage.MapStringMsgEntry](#basic_test-MapMessage-MapStringMsgEntry)
    - [MapMessageWireEquiv](#basic_test-MapMessageWireEquiv)
    - [MapMessageWireEquiv_entry1](#basic_test-MapMessageWireEquiv_entry1)
    - [MapMessageWireEquiv_entry2](#basic_test-MapMessageWireEquiv_entry2)
    - [MyRepeatedStruct](#basic_test-MyRepeatedStruct)
    - [MyStruct](#basic_test-MyStruct)
    - [OneofMessage](#basic_test-OneofMessage)
    - [Outer](#basic_test-Outer)
    - [Outer.ItemsEntry](#basic_test-Outer-ItemsEntry)
    - [Recursive1](#basic_test-Recursive1)
    - [Recursive2](#basic_test-Recursive2)
    - [TestEmbeddedMessageChild](#basic_test-TestEmbeddedMessageChild)
    - [TestEmbeddedMessageParent](#basic_test-TestEmbeddedMessageParent)
    - [TestMessage](#basic_test-TestMessage)
    - [TestMessage2](#basic_test-TestMessage2)
    - [TestSingularFields](#basic_test-TestSingularFields)
    - [TimeMessage](#basic_test-TimeMessage)
    - [WithJsonName](#basic_test-WithJsonName)
    - [Wrapper](#basic_test-Wrapper)
    - [Wrapper.MapBoolEntry](#basic_test-Wrapper-MapBoolEntry)
    - [Wrapper.MapBytesEntry](#basic_test-Wrapper-MapBytesEntry)
    - [Wrapper.MapDoubleEntry](#basic_test-Wrapper-MapDoubleEntry)
    - [Wrapper.MapFloatEntry](#basic_test-Wrapper-MapFloatEntry)
    - [Wrapper.MapInt32Entry](#basic_test-Wrapper-MapInt32Entry)
    - [Wrapper.MapInt64Entry](#basic_test-Wrapper-MapInt64Entry)
    - [Wrapper.MapStringEntry](#basic_test-Wrapper-MapStringEntry)
    - [Wrapper.MapUint32Entry](#basic_test-Wrapper-MapUint32Entry)
    - [Wrapper.MapUint64Entry](#basic_test-Wrapper-MapUint64Entry)
  
    - [TestEnum](#basic_test-TestEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="ruby_tests_basic_test-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## ruby/tests/basic_test.proto



<a name="basic_test-Bar"></a>

### Bar



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| msg | [string](#string) |  |  |






<a name="basic_test-Baz"></a>

### Baz



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| msg | [string](#string) |  |  |






<a name="basic_test-Enumer"></a>

### Enumer



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_enum | [TestEnum](#basic_test-TestEnum) |  |  |
| repeated_enum | [TestEnum](#basic_test-TestEnum) | repeated |  |
| a_const | [string](#string) |  |  |
| str | [string](#string) |  |  |
| const | [TestEnum](#basic_test-TestEnum) |  |  |






<a name="basic_test-Foo"></a>

### Foo



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bar | [Bar](#basic_test-Bar) |  |  |
| baz | [Baz](#basic_test-Baz) | repeated |  |






<a name="basic_test-HelloRequest"></a>

### HelloRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) | optional |  |
| random_name_a0 | [uint32](#uint32) | optional |  |
| random_name_a1 | [uint32](#uint32) | optional |  |
| random_name_a2 | [uint32](#uint32) | optional |  |
| random_name_a3 | [uint32](#uint32) | optional |  |
| random_name_a4 | [uint32](#uint32) | optional |  |
| random_name_a5 | [uint32](#uint32) | optional |  |
| random_name_a6 | [uint32](#uint32) | optional |  |
| random_name_a7 | [uint32](#uint32) | optional |  |
| random_name_a8 | [uint32](#uint32) | optional |  |
| random_name_a9 | [uint32](#uint32) | optional |  |
| random_name_b0 | [uint32](#uint32) | optional |  |
| random_name_b1 | [uint32](#uint32) | optional |  |
| random_name_b2 | [uint32](#uint32) | optional |  |
| random_name_b3 | [uint32](#uint32) | optional |  |
| random_name_b4 | [uint32](#uint32) | optional |  |
| random_name_b5 | [uint32](#uint32) | optional |  |
| random_name_b6 | [uint32](#uint32) | optional |  |
| random_name_b7 | [uint32](#uint32) | optional |  |
| random_name_b8 | [uint32](#uint32) | optional |  |
| random_name_b9 | [uint32](#uint32) | optional |  |
| random_name_c0 | [uint32](#uint32) | optional |  |
| random_name_c1 | [uint32](#uint32) | optional |  |
| random_name_c2 | [uint32](#uint32) | optional |  |
| random_name_c3 | [uint32](#uint32) | optional |  |
| random_name_c4 | [uint32](#uint32) | optional |  |
| random_name_c5 | [uint32](#uint32) | optional |  |
| random_name_c6 | [uint32](#uint32) | optional |  |
| random_name_c7 | [uint32](#uint32) | optional |  |
| random_name_c8 | [uint32](#uint32) | optional |  |
| random_name_c9 | [uint32](#uint32) | optional |  |
| version | [string](#string) | optional |  |






<a name="basic_test-Inner"></a>

### Inner







<a name="basic_test-MapMessage"></a>

### MapMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map_string_int32 | [MapMessage.MapStringInt32Entry](#basic_test-MapMessage-MapStringInt32Entry) | repeated |  |
| map_string_msg | [MapMessage.MapStringMsgEntry](#basic_test-MapMessage-MapStringMsgEntry) | repeated |  |
| map_string_enum | [MapMessage.MapStringEnumEntry](#basic_test-MapMessage-MapStringEnumEntry) | repeated |  |






<a name="basic_test-MapMessage-MapStringEnumEntry"></a>

### MapMessage.MapStringEnumEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [TestEnum](#basic_test-TestEnum) |  |  |






<a name="basic_test-MapMessage-MapStringInt32Entry"></a>

### MapMessage.MapStringInt32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="basic_test-MapMessage-MapStringMsgEntry"></a>

### MapMessage.MapStringMsgEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [TestMessage2](#basic_test-TestMessage2) |  |  |






<a name="basic_test-MapMessageWireEquiv"></a>

### MapMessageWireEquiv



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| map_string_int32 | [MapMessageWireEquiv_entry1](#basic_test-MapMessageWireEquiv_entry1) | repeated |  |
| map_string_msg | [MapMessageWireEquiv_entry2](#basic_test-MapMessageWireEquiv_entry2) | repeated |  |






<a name="basic_test-MapMessageWireEquiv_entry1"></a>

### MapMessageWireEquiv_entry1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="basic_test-MapMessageWireEquiv_entry2"></a>

### MapMessageWireEquiv_entry2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [TestMessage2](#basic_test-TestMessage2) |  |  |






<a name="basic_test-MyRepeatedStruct"></a>

### MyRepeatedStruct



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| structs | [MyStruct](#basic_test-MyStruct) | repeated |  |






<a name="basic_test-MyStruct"></a>

### MyStruct



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| string | [string](#string) |  |  |
| struct | [google.protobuf.Struct](#google-protobuf-Struct) |  |  |






<a name="basic_test-OneofMessage"></a>

### OneofMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [string](#string) |  |  |
| b | [int32](#int32) |  |  |
| c | [TestMessage2](#basic_test-TestMessage2) |  |  |
| d | [TestEnum](#basic_test-TestEnum) |  |  |






<a name="basic_test-Outer"></a>

### Outer



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [Outer.ItemsEntry](#basic_test-Outer-ItemsEntry) | repeated |  |






<a name="basic_test-Outer-ItemsEntry"></a>

### Outer.ItemsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [Inner](#basic_test-Inner) |  |  |






<a name="basic_test-Recursive1"></a>

### Recursive1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [Recursive2](#basic_test-Recursive2) |  |  |






<a name="basic_test-Recursive2"></a>

### Recursive2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [Recursive1](#basic_test-Recursive1) |  |  |






<a name="basic_test-TestEmbeddedMessageChild"></a>

### TestEmbeddedMessageChild



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| sub_child | [TestMessage](#basic_test-TestMessage) |  |  |






<a name="basic_test-TestEmbeddedMessageParent"></a>

### TestEmbeddedMessageParent



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| child_msg | [TestEmbeddedMessageChild](#basic_test-TestEmbeddedMessageChild) |  |  |
| number | [int32](#int32) |  |  |
| repeated_msg | [TestEmbeddedMessageChild](#basic_test-TestEmbeddedMessageChild) | repeated |  |
| repeated_number | [int32](#int32) | repeated |  |






<a name="basic_test-TestMessage"></a>

### TestMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) | optional |  |
| optional_int64 | [int64](#int64) | optional |  |
| optional_uint32 | [uint32](#uint32) | optional |  |
| optional_uint64 | [uint64](#uint64) | optional |  |
| optional_bool | [bool](#bool) | optional |  |
| optional_float | [float](#float) | optional |  |
| optional_double | [double](#double) | optional |  |
| optional_string | [string](#string) | optional |  |
| optional_bytes | [bytes](#bytes) | optional |  |
| optional_msg | [TestMessage2](#basic_test-TestMessage2) | optional |  |
| optional_enum | [TestEnum](#basic_test-TestEnum) | optional |  |
| repeated_int32 | [int32](#int32) | repeated |  |
| repeated_int64 | [int64](#int64) | repeated |  |
| repeated_uint32 | [uint32](#uint32) | repeated |  |
| repeated_uint64 | [uint64](#uint64) | repeated |  |
| repeated_bool | [bool](#bool) | repeated |  |
| repeated_float | [float](#float) | repeated |  |
| repeated_double | [double](#double) | repeated |  |
| repeated_string | [string](#string) | repeated |  |
| repeated_bytes | [bytes](#bytes) | repeated |  |
| repeated_msg | [TestMessage2](#basic_test-TestMessage2) | repeated |  |
| repeated_enum | [TestEnum](#basic_test-TestEnum) | repeated |  |
| optional_msg2 | [TestSingularFields](#basic_test-TestSingularFields) | optional |  |






<a name="basic_test-TestMessage2"></a>

### TestMessage2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [int32](#int32) | optional |  |






<a name="basic_test-TestSingularFields"></a>

### TestSingularFields



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| singular_int32 | [int32](#int32) |  |  |
| singular_int64 | [int64](#int64) |  |  |
| singular_uint32 | [uint32](#uint32) |  |  |
| singular_uint64 | [uint64](#uint64) |  |  |
| singular_bool | [bool](#bool) |  |  |
| singular_float | [float](#float) |  |  |
| singular_double | [double](#double) |  |  |
| singular_string | [string](#string) |  |  |
| singular_bytes | [bytes](#bytes) |  |  |
| singular_msg | [TestMessage2](#basic_test-TestMessage2) |  |  |
| singular_enum | [TestEnum](#basic_test-TestEnum) |  |  |






<a name="basic_test-TimeMessage"></a>

### TimeMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| timestamp | [google.protobuf.Timestamp](#google-protobuf-Timestamp) |  |  |
| duration | [google.protobuf.Duration](#google-protobuf-Duration) |  |  |






<a name="basic_test-WithJsonName"></a>

### WithJsonName



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo_bar | [int32](#int32) | optional |  |
| baz | [WithJsonName](#basic_test-WithJsonName) | repeated |  |






<a name="basic_test-Wrapper"></a>

### Wrapper



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| double | [google.protobuf.DoubleValue](#google-protobuf-DoubleValue) |  |  |
| float | [google.protobuf.FloatValue](#google-protobuf-FloatValue) |  |  |
| int32 | [google.protobuf.Int32Value](#google-protobuf-Int32Value) |  |  |
| int64 | [google.protobuf.Int64Value](#google-protobuf-Int64Value) |  |  |
| uint32 | [google.protobuf.UInt32Value](#google-protobuf-UInt32Value) |  |  |
| uint64 | [google.protobuf.UInt64Value](#google-protobuf-UInt64Value) |  |  |
| bool | [google.protobuf.BoolValue](#google-protobuf-BoolValue) |  |  |
| string | [google.protobuf.StringValue](#google-protobuf-StringValue) |  |  |
| bytes | [google.protobuf.BytesValue](#google-protobuf-BytesValue) |  |  |
| real_string | [string](#string) |  |  |
| string_in_oneof | [string](#string) |  |  |
| repeated_double | [google.protobuf.DoubleValue](#google-protobuf-DoubleValue) | repeated | Repeated wrappers don&#39;t make sense, but we still need to make sure they work and don&#39;t crash. |
| repeated_float | [google.protobuf.FloatValue](#google-protobuf-FloatValue) | repeated |  |
| repeated_int32 | [google.protobuf.Int32Value](#google-protobuf-Int32Value) | repeated |  |
| repeated_int64 | [google.protobuf.Int64Value](#google-protobuf-Int64Value) | repeated |  |
| repeated_uint32 | [google.protobuf.UInt32Value](#google-protobuf-UInt32Value) | repeated |  |
| repeated_uint64 | [google.protobuf.UInt64Value](#google-protobuf-UInt64Value) | repeated |  |
| repeated_bool | [google.protobuf.BoolValue](#google-protobuf-BoolValue) | repeated |  |
| repeated_string | [google.protobuf.StringValue](#google-protobuf-StringValue) | repeated |  |
| repeated_bytes | [google.protobuf.BytesValue](#google-protobuf-BytesValue) | repeated |  |
| map_double | [Wrapper.MapDoubleEntry](#basic_test-Wrapper-MapDoubleEntry) | repeated | Wrappers as map keys don&#39;t make sense, but we still need to make sure they work and don&#39;t crash. |
| map_float | [Wrapper.MapFloatEntry](#basic_test-Wrapper-MapFloatEntry) | repeated |  |
| map_int32 | [Wrapper.MapInt32Entry](#basic_test-Wrapper-MapInt32Entry) | repeated |  |
| map_int64 | [Wrapper.MapInt64Entry](#basic_test-Wrapper-MapInt64Entry) | repeated |  |
| map_uint32 | [Wrapper.MapUint32Entry](#basic_test-Wrapper-MapUint32Entry) | repeated |  |
| map_uint64 | [Wrapper.MapUint64Entry](#basic_test-Wrapper-MapUint64Entry) | repeated |  |
| map_bool | [Wrapper.MapBoolEntry](#basic_test-Wrapper-MapBoolEntry) | repeated |  |
| map_string | [Wrapper.MapStringEntry](#basic_test-Wrapper-MapStringEntry) | repeated |  |
| map_bytes | [Wrapper.MapBytesEntry](#basic_test-Wrapper-MapBytesEntry) | repeated |  |
| oneof_double | [google.protobuf.DoubleValue](#google-protobuf-DoubleValue) |  |  |
| oneof_float | [google.protobuf.FloatValue](#google-protobuf-FloatValue) |  |  |
| oneof_int32 | [google.protobuf.Int32Value](#google-protobuf-Int32Value) |  |  |
| oneof_int64 | [google.protobuf.Int64Value](#google-protobuf-Int64Value) |  |  |
| oneof_uint32 | [google.protobuf.UInt32Value](#google-protobuf-UInt32Value) |  |  |
| oneof_uint64 | [google.protobuf.UInt64Value](#google-protobuf-UInt64Value) |  |  |
| oneof_bool | [google.protobuf.BoolValue](#google-protobuf-BoolValue) |  |  |
| oneof_string | [google.protobuf.StringValue](#google-protobuf-StringValue) |  |  |
| oneof_bytes | [google.protobuf.BytesValue](#google-protobuf-BytesValue) |  |  |
| oneof_plain_string | [string](#string) |  |  |






<a name="basic_test-Wrapper-MapBoolEntry"></a>

### Wrapper.MapBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.BoolValue](#google-protobuf-BoolValue) |  |  |






<a name="basic_test-Wrapper-MapBytesEntry"></a>

### Wrapper.MapBytesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.BytesValue](#google-protobuf-BytesValue) |  |  |






<a name="basic_test-Wrapper-MapDoubleEntry"></a>

### Wrapper.MapDoubleEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.DoubleValue](#google-protobuf-DoubleValue) |  |  |






<a name="basic_test-Wrapper-MapFloatEntry"></a>

### Wrapper.MapFloatEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.FloatValue](#google-protobuf-FloatValue) |  |  |






<a name="basic_test-Wrapper-MapInt32Entry"></a>

### Wrapper.MapInt32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.Int32Value](#google-protobuf-Int32Value) |  |  |






<a name="basic_test-Wrapper-MapInt64Entry"></a>

### Wrapper.MapInt64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.Int64Value](#google-protobuf-Int64Value) |  |  |






<a name="basic_test-Wrapper-MapStringEntry"></a>

### Wrapper.MapStringEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.StringValue](#google-protobuf-StringValue) |  |  |






<a name="basic_test-Wrapper-MapUint32Entry"></a>

### Wrapper.MapUint32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.UInt32Value](#google-protobuf-UInt32Value) |  |  |






<a name="basic_test-Wrapper-MapUint64Entry"></a>

### Wrapper.MapUint64Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [google.protobuf.UInt64Value](#google-protobuf-UInt64Value) |  |  |





 


<a name="basic_test-TestEnum"></a>

### TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| Default | 0 |  |
| A | 1 |  |
| B | 2 |  |
| C | 3 |  |
| v0 | 4 |  |


 

 

 



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

