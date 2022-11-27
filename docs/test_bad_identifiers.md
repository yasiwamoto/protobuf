# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [src/google/protobuf/compiler/cpp/test_bad_identifiers.proto](#src_google_protobuf_compiler_cpp_test_bad_identifiers-proto)
    - [DummyMessage](#protobuf_unittest-DummyMessage)
    - [NULL](#protobuf_unittest-NULL)
    - [Shutdown](#protobuf_unittest-Shutdown)
    - [TableStruct](#protobuf_unittest-TableStruct)
    - [TestConflictingEnumNames](#protobuf_unittest-TestConflictingEnumNames)
    - [TestConflictingSymbolNames](#protobuf_unittest-TestConflictingSymbolNames)
    - [TestConflictingSymbolNames.BuildDescriptors](#protobuf_unittest-TestConflictingSymbolNames-BuildDescriptors)
    - [TestConflictingSymbolNames.Cord](#protobuf_unittest-TestConflictingSymbolNames-Cord)
    - [TestConflictingSymbolNames.DO](#protobuf_unittest-TestConflictingSymbolNames-DO)
    - [TestConflictingSymbolNames.Data1](#protobuf_unittest-TestConflictingSymbolNames-Data1)
    - [TestConflictingSymbolNames.Data2](#protobuf_unittest-TestConflictingSymbolNames-Data2)
    - [TestConflictingSymbolNames.Data3](#protobuf_unittest-TestConflictingSymbolNames-Data3)
    - [TestConflictingSymbolNames.Data4](#protobuf_unittest-TestConflictingSymbolNames-Data4)
    - [TestConflictingSymbolNames.Data5](#protobuf_unittest-TestConflictingSymbolNames-Data5)
    - [TestConflictingSymbolNames.Data6](#protobuf_unittest-TestConflictingSymbolNames-Data6)
    - [TestConflictingSymbolNames.StringPiece](#protobuf_unittest-TestConflictingSymbolNames-StringPiece)
    - [TestConflictingSymbolNames.TypeTraits](#protobuf_unittest-TestConflictingSymbolNames-TypeTraits)
    - [TestConflictingSymbolNamesExtension](#protobuf_unittest-TestConflictingSymbolNamesExtension)
  
    - [TestConflictingEnumNames.while](#protobuf_unittest-TestConflictingEnumNames-while)
    - [TestConflictingSymbolNames.TestEnum](#protobuf_unittest-TestConflictingSymbolNames-TestEnum)
    - [bool](#protobuf_unittest-bool)
  
    - [File-level Extensions](#src_google_protobuf_compiler_cpp_test_bad_identifiers-proto-extensions)
  
    - [TestConflictingMethodNames](#protobuf_unittest-TestConflictingMethodNames)
  
- [Scalar Value Types](#scalar-value-types)



<a name="src_google_protobuf_compiler_cpp_test_bad_identifiers-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## src/google/protobuf/compiler/cpp/test_bad_identifiers.proto



<a name="protobuf_unittest-DummyMessage"></a>

### DummyMessage







<a name="protobuf_unittest-NULL"></a>

### NULL



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| int | [int32](#int32) | optional |  |






<a name="protobuf_unittest-Shutdown"></a>

### Shutdown
Message names that could conflict.






<a name="protobuf_unittest-TableStruct"></a>

### TableStruct







<a name="protobuf_unittest-TestConflictingEnumNames"></a>

### TestConflictingEnumNames
NO_PROTO3


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| conflicting_enum | [TestConflictingEnumNames.while](#protobuf_unittest-TestConflictingEnumNames-while) | optional | NO_PROTO3 |






<a name="protobuf_unittest-TestConflictingSymbolNames"></a>

### TestConflictingSymbolNames
Test that fields can have names like &#34;input&#34; and &#34;i&#34; which are also used
internally by the code generator for local variables.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| input | [int32](#int32) | optional |  |
| output | [int32](#int32) | optional |  |
| length | [string](#string) | optional |  |
| i | [int32](#int32) | repeated |  |
| new_element | [string](#string) | repeated |  |
| total_size | [int32](#int32) | optional |  |
| tag | [int32](#int32) | optional |  |
| source | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |
| file | [int32](#int32) | optional |  |
| from | [int32](#int32) | optional |  |
| handle_uninterpreted | [int32](#int32) | optional |  |
| index | [int32](#int32) | repeated |  |
| controller | [int32](#int32) | optional |  |
| already_here | [int32](#int32) | optional |  |
| uint32 | [uint32](#uint32) | optional |  |
| uint32_t | [uint32](#uint32) | optional |  |
| uint64 | [uint64](#uint64) | optional |  |
| uint64_t | [uint32](#uint32) | optional |  |
| string | [string](#string) | optional |  |
| memset | [int32](#int32) | optional |  |
| int32 | [int32](#int32) | optional |  |
| int32_t | [int32](#int32) | optional |  |
| int64 | [int64](#int64) | optional |  |
| int64_t | [int64](#int64) | optional |  |
| size_t | [int64](#int64) | optional |  |
| cached_size | [uint32](#uint32) | optional |  |
| extensions | [uint32](#uint32) | optional |  |
| bit | [uint32](#uint32) | optional |  |
| bits | [uint32](#uint32) | optional |  |
| offsets | [uint32](#uint32) | optional |  |
| reflection | [uint32](#uint32) | optional |  |
| some_cord | [string](#string) | optional |  |
| some_string_piece | [string](#string) | optional |  |
| int | [uint32](#uint32) | optional | Some keywords. |
| friend | [uint32](#uint32) | optional |  |
| class | [uint32](#uint32) | optional |  |
| typedecl | [uint32](#uint32) | optional |  |
| auto | [uint32](#uint32) | optional |  |
| do | [TestConflictingSymbolNames.DO](#protobuf_unittest-TestConflictingSymbolNames-DO) | optional |  |
| field_type | [int32](#int32) | optional | Some template parameter names for extensions. |
| is_packed | [bool](#bool) | optional |  |
| release_length | [string](#string) | optional | test conflicting release_$name$. &#34;length&#34; and &#34;do&#34; field in this message must remain string or message fields to make the test valid. |
| release_do | [TestConflictingSymbolNames.DO](#protobuf_unittest-TestConflictingSymbolNames-DO) | optional | A more extreme case, the field name &#34;do&#34; here is a keyword, which will be escaped to &#34;do_&#34; already. Test there is no conflict even with escaped field names. |
| target | [string](#string) | optional | For clashing local variables in Serialize and ByteSize calculation. |






<a name="protobuf_unittest-TestConflictingSymbolNames-BuildDescriptors"></a>

### TestConflictingSymbolNames.BuildDescriptors







<a name="protobuf_unittest-TestConflictingSymbolNames-Cord"></a>

### TestConflictingSymbolNames.Cord







<a name="protobuf_unittest-TestConflictingSymbolNames-DO"></a>

### TestConflictingSymbolNames.DO
The generator used to #define a macro called &#34;DO&#34; inside the .cc file.






<a name="protobuf_unittest-TestConflictingSymbolNames-Data1"></a>

### TestConflictingSymbolNames.Data1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [int32](#int32) | repeated |  |






<a name="protobuf_unittest-TestConflictingSymbolNames-Data2"></a>

### TestConflictingSymbolNames.Data2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [TestConflictingSymbolNames.TestEnum](#protobuf_unittest-TestConflictingSymbolNames-TestEnum) | repeated |  |






<a name="protobuf_unittest-TestConflictingSymbolNames-Data3"></a>

### TestConflictingSymbolNames.Data3



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [string](#string) | repeated |  |






<a name="protobuf_unittest-TestConflictingSymbolNames-Data4"></a>

### TestConflictingSymbolNames.Data4



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [TestConflictingSymbolNames.Data4](#protobuf_unittest-TestConflictingSymbolNames-Data4) | repeated |  |






<a name="protobuf_unittest-TestConflictingSymbolNames-Data5"></a>

### TestConflictingSymbolNames.Data5



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [string](#string) | repeated |  |






<a name="protobuf_unittest-TestConflictingSymbolNames-Data6"></a>

### TestConflictingSymbolNames.Data6



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [string](#string) | repeated |  |






<a name="protobuf_unittest-TestConflictingSymbolNames-StringPiece"></a>

### TestConflictingSymbolNames.StringPiece







<a name="protobuf_unittest-TestConflictingSymbolNames-TypeTraits"></a>

### TestConflictingSymbolNames.TypeTraits







<a name="protobuf_unittest-TestConflictingSymbolNamesExtension"></a>

### TestConflictingSymbolNamesExtension
NO_PROTO3




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| repeated_int32_ext | int32 | TestConflictingSymbolNames | 20423638 | NO_PROTO3 |



 


<a name="protobuf_unittest-TestConflictingEnumNames-while"></a>

### TestConflictingEnumNames.while
NO_PROTO3

| Name | Number | Description |
| ---- | ------ | ----------- |
| default | 0 | NO_PROTO3 |
| and | 1 | NO_PROTO3 |
| class | 2 | NO_PROTO3 |
| int | 3 | NO_PROTO3 |
| typedef | 4 | NO_PROTO3 |
| XOR | 5 | NO_PROTO3 |



<a name="protobuf_unittest-TestConflictingSymbolNames-TestEnum"></a>

### TestConflictingSymbolNames.TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 0 |  |



<a name="protobuf_unittest-bool"></a>

### bool
NO_PROTO3

| Name | Number | Description |
| ---- | ------ | ----------- |
| default | 0 | NO_PROTO3 |
| NOT_EQ | 1 | NO_PROTO3 |
| volatile | 2 | NO_PROTO3 |
| return | 3 | NO_PROTO3 |


 


<a name="src_google_protobuf_compiler_cpp_test_bad_identifiers-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| void | int32 | TestConflictingSymbolNames | 314253 | NO_PROTO3 |

 


<a name="protobuf_unittest-TestConflictingMethodNames"></a>

### TestConflictingMethodNames


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| Closure | [DummyMessage](#protobuf_unittest-DummyMessage) | [DummyMessage](#protobuf_unittest-DummyMessage) |  |

 



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

