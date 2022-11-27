# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_objc_options.proto](#objectivec_Tests_unittest_objc_options-proto)
    - [GPBTEST](#objc-protobuf-tests-options-GPBTEST)
    - [GPBTESTTestHasAPrefixMessage](#objc-protobuf-tests-options-GPBTESTTestHasAPrefixMessage)
    - [GPBTESTshouldGetAPrefixMessage](#objc-protobuf-tests-options-GPBTESTshouldGetAPrefixMessage)
    - [PrefixedParentMessage](#objc-protobuf-tests-options-PrefixedParentMessage)
    - [PrefixedParentMessage.Child](#objc-protobuf-tests-options-PrefixedParentMessage-Child)
    - [TestObjcProtoPrefixMessage](#objc-protobuf-tests-options-TestObjcProtoPrefixMessage)
  
    - [GPBTESTTestHasAPrefixEnum](#objc-protobuf-tests-options-GPBTESTTestHasAPrefixEnum)
    - [TestObjcProtoPrefixEnum](#objc-protobuf-tests-options-TestObjcProtoPrefixEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_objc_options-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_objc_options.proto



<a name="objc-protobuf-tests-options-GPBTEST"></a>

### GPBTEST
Verify that classes named the same as prefixes are prefixed.






<a name="objc-protobuf-tests-options-GPBTESTTestHasAPrefixMessage"></a>

### GPBTESTTestHasAPrefixMessage
Verify that messages that already have a prefix aren&#39;t prefixed twice.






<a name="objc-protobuf-tests-options-GPBTESTshouldGetAPrefixMessage"></a>

### GPBTESTshouldGetAPrefixMessage
Verify that classes that have the prefix followed by a lowercase
letter DO get the prefix.






<a name="objc-protobuf-tests-options-PrefixedParentMessage"></a>

### PrefixedParentMessage
Tests that lookup deals with prefix.






<a name="objc-protobuf-tests-options-PrefixedParentMessage-Child"></a>

### PrefixedParentMessage.Child







<a name="objc-protobuf-tests-options-TestObjcProtoPrefixMessage"></a>

### TestObjcProtoPrefixMessage
Verify that enum types and values get the prefix.





 


<a name="objc-protobuf-tests-options-GPBTESTTestHasAPrefixEnum"></a>

### GPBTESTTestHasAPrefixEnum
Verify that enums that already have a prefix aren&#39;t prefixed twice.

| Name | Number | Description |
| ---- | ------ | ----------- |
| valueB | 1 |  |



<a name="objc-protobuf-tests-options-TestObjcProtoPrefixEnum"></a>

### TestObjcProtoPrefixEnum
Verify that messages that don&#39;t already have the prefix get a prefix.

| Name | Number | Description |
| ---- | ------ | ----------- |
| value | 1 |  |


 

 

 



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

