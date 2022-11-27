# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_mset.proto](#objectivec_Tests_unittest_mset-proto)
    - [Message](#objc-protobuf-tests-mset-Message)
    - [MessageExtension1](#objc-protobuf-tests-mset-MessageExtension1)
    - [MessageExtension2](#objc-protobuf-tests-mset-MessageExtension2)
    - [RawMessageSet](#objc-protobuf-tests-mset-RawMessageSet)
    - [RawMessageSet.Item](#objc-protobuf-tests-mset-RawMessageSet-Item)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_mset-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_mset.proto



<a name="objc-protobuf-tests-mset-Message"></a>

### Message
A message with message_set_wire_format.






<a name="objc-protobuf-tests-mset-MessageExtension1"></a>

### MessageExtension1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| i | [int32](#int32) | optional |  |
| recursive | [Message](#objc-protobuf-tests-mset-Message) | optional |  |
| test_aliasing | [string](#string) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| message_set_extension | MessageExtension1 | Message | 1545008 |  |




<a name="objc-protobuf-tests-mset-MessageExtension2"></a>

### MessageExtension2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| str | [string](#string) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| message_set_extension | MessageExtension2 | Message | 1547769 |  |




<a name="objc-protobuf-tests-mset-RawMessageSet"></a>

### RawMessageSet
MessageSet wire format is equivalent to this.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item | [RawMessageSet.Item](#objc-protobuf-tests-mset-RawMessageSet-Item) | repeated |  |






<a name="objc-protobuf-tests-mset-RawMessageSet-Item"></a>

### RawMessageSet.Item



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type_id | [int32](#int32) | required |  |
| message | [bytes](#bytes) | required |  |





 

 

 

 



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

