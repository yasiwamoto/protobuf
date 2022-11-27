# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [python/google/protobuf/internal/factory_test1.proto](#python_google_protobuf_internal_factory_test1-proto)
    - [Factory1Message](#google-protobuf-python-internal-Factory1Message)
    - [Factory1Message.NestedFactory1Message](#google-protobuf-python-internal-Factory1Message-NestedFactory1Message)
    - [Factory1MethodRequest](#google-protobuf-python-internal-Factory1MethodRequest)
    - [Factory1MethodResponse](#google-protobuf-python-internal-Factory1MethodResponse)
  
    - [Factory1Enum](#google-protobuf-python-internal-Factory1Enum)
    - [Factory1Message.NestedFactory1Enum](#google-protobuf-python-internal-Factory1Message-NestedFactory1Enum)
  
    - [Factory1Service](#google-protobuf-python-internal-Factory1Service)
  
- [Scalar Value Types](#scalar-value-types)



<a name="python_google_protobuf_internal_factory_test1-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## python/google/protobuf/internal/factory_test1.proto



<a name="google-protobuf-python-internal-Factory1Message"></a>

### Factory1Message



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| factory_1_enum | [Factory1Enum](#google-protobuf-python-internal-Factory1Enum) | optional |  |
| nested_factory_1_enum | [Factory1Message.NestedFactory1Enum](#google-protobuf-python-internal-Factory1Message-NestedFactory1Enum) | optional |  |
| nested_factory_1_message | [Factory1Message.NestedFactory1Message](#google-protobuf-python-internal-Factory1Message-NestedFactory1Message) | optional |  |
| scalar_value | [int32](#int32) | optional |  |
| list_value | [string](#string) | repeated |  |






<a name="google-protobuf-python-internal-Factory1Message-NestedFactory1Message"></a>

### Factory1Message.NestedFactory1Message



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [string](#string) | optional |  |






<a name="google-protobuf-python-internal-Factory1MethodRequest"></a>

### Factory1MethodRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| argument | [string](#string) | optional |  |






<a name="google-protobuf-python-internal-Factory1MethodResponse"></a>

### Factory1MethodResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| result | [string](#string) | optional |  |





 


<a name="google-protobuf-python-internal-Factory1Enum"></a>

### Factory1Enum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FACTORY_1_VALUE_0 | 0 |  |
| FACTORY_1_VALUE_1 | 1 |  |



<a name="google-protobuf-python-internal-Factory1Message-NestedFactory1Enum"></a>

### Factory1Message.NestedFactory1Enum


| Name | Number | Description |
| ---- | ------ | ----------- |
| NESTED_FACTORY_1_VALUE_0 | 0 |  |
| NESTED_FACTORY_1_VALUE_1 | 1 |  |


 

 


<a name="google-protobuf-python-internal-Factory1Service"></a>

### Factory1Service


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| Factory1Method | [Factory1MethodRequest](#google-protobuf-python-internal-Factory1MethodRequest) | [Factory1MethodResponse](#google-protobuf-python-internal-Factory1MethodResponse) | Dummy method for this dummy service. |

 



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

