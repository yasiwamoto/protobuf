# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [python/google/protobuf/internal/test_proto3_optional.proto](#python_google_protobuf_internal_test_proto3_optional-proto)
    - [TestProto3Optional](#google-protobuf-python-internal-TestProto3Optional)
    - [TestProto3Optional.NestedMessage](#google-protobuf-python-internal-TestProto3Optional-NestedMessage)
  
    - [TestProto3Optional.NestedEnum](#google-protobuf-python-internal-TestProto3Optional-NestedEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="python_google_protobuf_internal_test_proto3_optional-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## python/google/protobuf/internal/test_proto3_optional.proto



<a name="google-protobuf-python-internal-TestProto3Optional"></a>

### TestProto3Optional



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) | optional | Singular |
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
| optional_nested_message | [TestProto3Optional.NestedMessage](#google-protobuf-python-internal-TestProto3Optional-NestedMessage) | optional |  |
| optional_nested_enum | [TestProto3Optional.NestedEnum](#google-protobuf-python-internal-TestProto3Optional-NestedEnum) | optional |  |






<a name="google-protobuf-python-internal-TestProto3Optional-NestedMessage"></a>

### TestProto3Optional.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bb | [int32](#int32) | optional | The field name &#34;b&#34; fails to compile in proto1 because it conflicts with a local variable named &#34;b&#34; in one of the generated methods. Doh. This file needs to compile in proto1 to test backwards-compatibility. |





 


<a name="google-protobuf-python-internal-TestProto3Optional-NestedEnum"></a>

### TestProto3Optional.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNSPECIFIED | 0 |  |
| FOO | 1 |  |
| BAR | 2 |  |
| BAZ | 3 |  |
| NEG | -1 | Intentionally negative. |


 

 

 



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

