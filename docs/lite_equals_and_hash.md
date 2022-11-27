# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/core/src/test/proto/com/google/protobuf/lite_equals_and_hash.proto](#java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto)
    - [Bar](#protobuf_unittest-lite_equals_and_hash-Bar)
    - [BarPrime](#protobuf_unittest-lite_equals_and_hash-BarPrime)
    - [Empty](#protobuf_unittest-lite_equals_and_hash-Empty)
    - [Foo](#protobuf_unittest-lite_equals_and_hash-Foo)
    - [Foo.MyGroup](#protobuf_unittest-lite_equals_and_hash-Foo-MyGroup)
    - [Foo.MyMapEntry](#protobuf_unittest-lite_equals_and_hash-Foo-MyMapEntry)
    - [MyGroup](#protobuf_unittest-lite_equals_and_hash-MyGroup)
    - [TestOneofEquals](#protobuf_unittest-lite_equals_and_hash-TestOneofEquals)
    - [TestRecursiveOneof](#protobuf_unittest-lite_equals_and_hash-TestRecursiveOneof)
  
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/core/src/test/proto/com/google/protobuf/lite_equals_and_hash.proto



<a name="protobuf_unittest-lite_equals_and_hash-Bar"></a>

### Bar



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| foo_ext | Bar | Foo | 100 |  |




<a name="protobuf_unittest-lite_equals_and_hash-BarPrime"></a>

### BarPrime



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) | optional |  |






<a name="protobuf_unittest-lite_equals_and_hash-Empty"></a>

### Empty







<a name="protobuf_unittest-lite_equals_and_hash-Foo"></a>

### Foo



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) | optional |  |
| bar | [Bar](#protobuf_unittest-lite_equals_and_hash-Bar) | repeated |  |
| my_map | [Foo.MyMapEntry](#protobuf_unittest-lite_equals_and_hash-Foo-MyMapEntry) | repeated |  |
| sint64 | [sint64](#sint64) | optional |  |
| mygroup | [Foo.MyGroup](#protobuf_unittest-lite_equals_and_hash-Foo-MyGroup) | optional |  |






<a name="protobuf_unittest-lite_equals_and_hash-Foo-MyGroup"></a>

### Foo.MyGroup
LINT: ALLOW_GROUPS


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) | optional |  |






<a name="protobuf_unittest-lite_equals_and_hash-Foo-MyMapEntry"></a>

### Foo.MyMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf_unittest-lite_equals_and_hash-MyGroup"></a>

### MyGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_value | [string](#string) | optional |  |






<a name="protobuf_unittest-lite_equals_and_hash-TestOneofEquals"></a>

### TestOneofEquals



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf_unittest-lite_equals_and_hash-TestRecursiveOneof"></a>

### TestRecursiveOneof



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| r | [TestRecursiveOneof](#protobuf_unittest-lite_equals_and_hash-TestRecursiveOneof) | optional |  |





 

 


<a name="java_core_src_test_proto_com_google_protobuf_lite_equals_and_hash-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| fixed32 | fixed32 | Foo | 102 |  |
| fixed64 | fixed64 | Foo | 103 |  |
| mygroup | MyGroup | Foo | 104 |  |
| varint | int32 | Foo | 101 |  |

 

 



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

