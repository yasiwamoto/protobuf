# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [python/google/protobuf/internal/descriptor_pool_test1.proto](#python_google_protobuf_internal_descriptor_pool_test1-proto)
    - [DescriptorPoolTest1](#google-protobuf-python-internal-DescriptorPoolTest1)
    - [DescriptorPoolTest1.NestedMessage](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage)
    - [DescriptorPoolTest1.NestedMessage.DeepNestedMessage](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-DeepNestedMessage)
    - [DescriptorPoolTest2](#google-protobuf-python-internal-DescriptorPoolTest2)
    - [DescriptorPoolTest2.NestedMessage](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage)
    - [DescriptorPoolTest2.NestedMessage.DeepNestedMessage](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-DeepNestedMessage)
  
    - [DescriptorPoolTest1.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest1-NestedEnum)
    - [DescriptorPoolTest1.NestedMessage.DeepNestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-DeepNestedMessage-NestedEnum)
    - [DescriptorPoolTest1.NestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-NestedEnum)
    - [DescriptorPoolTest2.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest2-NestedEnum)
    - [DescriptorPoolTest2.NestedMessage.DeepNestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-DeepNestedMessage-NestedEnum)
    - [DescriptorPoolTest2.NestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-NestedEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="python_google_protobuf_internal_descriptor_pool_test1-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## python/google/protobuf/internal/descriptor_pool_test1.proto



<a name="google-protobuf-python-internal-DescriptorPoolTest1"></a>

### DescriptorPoolTest1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nested_enum | [DescriptorPoolTest1.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest1-NestedEnum) | optional |  Default: BETA |
| nested_message | [DescriptorPoolTest1.NestedMessage](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage) | optional |  |






<a name="google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage"></a>

### DescriptorPoolTest1.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nested_enum | [DescriptorPoolTest1.NestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-NestedEnum) | optional |  Default: ZETA |
| nested_field | [string](#string) | optional |  Default: beta |
| deep_nested_message | [DescriptorPoolTest1.NestedMessage.DeepNestedMessage](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-DeepNestedMessage) | optional |  |






<a name="google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-DeepNestedMessage"></a>

### DescriptorPoolTest1.NestedMessage.DeepNestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nested_enum | [DescriptorPoolTest1.NestedMessage.DeepNestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-DeepNestedMessage-NestedEnum) | optional |  Default: ETA |
| nested_field | [string](#string) | optional |  Default: theta |






<a name="google-protobuf-python-internal-DescriptorPoolTest2"></a>

### DescriptorPoolTest2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nested_enum | [DescriptorPoolTest2.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest2-NestedEnum) | optional |  Default: GAMMA |
| nested_message | [DescriptorPoolTest2.NestedMessage](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage) | optional |  |






<a name="google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage"></a>

### DescriptorPoolTest2.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nested_enum | [DescriptorPoolTest2.NestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-NestedEnum) | optional |  Default: IOTA |
| nested_field | [string](#string) | optional |  Default: delta |
| deep_nested_message | [DescriptorPoolTest2.NestedMessage.DeepNestedMessage](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-DeepNestedMessage) | optional |  |






<a name="google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-DeepNestedMessage"></a>

### DescriptorPoolTest2.NestedMessage.DeepNestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nested_enum | [DescriptorPoolTest2.NestedMessage.DeepNestedMessage.NestedEnum](#google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-DeepNestedMessage-NestedEnum) | optional |  Default: MU |
| nested_field | [string](#string) | optional |  Default: lambda |





 


<a name="google-protobuf-python-internal-DescriptorPoolTest1-NestedEnum"></a>

### DescriptorPoolTest1.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ALPHA | 1 |  |
| BETA | 2 |  |



<a name="google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-DeepNestedMessage-NestedEnum"></a>

### DescriptorPoolTest1.NestedMessage.DeepNestedMessage.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ETA | 7 |  |
| THETA | 8 |  |



<a name="google-protobuf-python-internal-DescriptorPoolTest1-NestedMessage-NestedEnum"></a>

### DescriptorPoolTest1.NestedMessage.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| EPSILON | 5 |  |
| ZETA | 6 |  |



<a name="google-protobuf-python-internal-DescriptorPoolTest2-NestedEnum"></a>

### DescriptorPoolTest2.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| GAMMA | 3 |  |
| DELTA | 4 |  |



<a name="google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-DeepNestedMessage-NestedEnum"></a>

### DescriptorPoolTest2.NestedMessage.DeepNestedMessage.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| LAMBDA | 11 |  |
| MU | 12 |  |



<a name="google-protobuf-python-internal-DescriptorPoolTest2-NestedMessage-NestedEnum"></a>

### DescriptorPoolTest2.NestedMessage.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| IOTA | 9 |  |
| KAPPA | 10 |  |


 

 

 



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

