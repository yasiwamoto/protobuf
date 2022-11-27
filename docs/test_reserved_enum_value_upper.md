# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [php/tests/proto/test_reserved_enum_value_upper.proto](#php_tests_proto_test_reserved_enum_value_upper-proto)
    - [NotAllowed](#upper_enum_value-NotAllowed)
  
- [Scalar Value Types](#scalar-value-types)



<a name="php_tests_proto_test_reserved_enum_value_upper-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## php/tests/proto/test_reserved_enum_value_upper.proto


 


<a name="upper_enum_value-NotAllowed"></a>

### NotAllowed


| Name | Number | Description |
| ---- | ------ | ----------- |
| ABSTRACT | 0 |  |
| AND | 1 |  |
| ARRAY | 2 |  |
| AS | 3 |  |
| BREAK | 4 |  |
| CALLABLE | 5 |  |
| CASE | 6 |  |
| CATCH | 7 |  |
| CLASS | 8 |  |
| CLONE | 9 |  |
| CONST | 10 |  |
| CONTINUE | 11 |  |
| DECLARE | 12 |  |
| DEFAULT | 13 |  |
| DIE | 14 |  |
| DO | 15 |  |
| ECHO | 16 |  |
| ELSE | 17 |  |
| ELSEIF | 18 |  |
| EMPTY | 19 |  |
| ENDDECLARE | 20 |  |
| ENDFOR | 21 |  |
| ENDFOREACH | 22 |  |
| ENDIF | 23 |  |
| ENDSWITCH | 24 |  |
| ENDWHILE | 25 |  |
| EVAL | 26 |  |
| EXIT | 27 |  |
| EXTENDS | 28 |  |
| FINAL | 29 |  |
| FINALLY | 30 |  |
| FOR | 31 |  |
| FOREACH | 32 |  |
| FUNCTION | 33 |  |
| FN | 34 |  |
| GLOBAL | 35 |  |
| GOTO | 36 |  |
| IF | 37 |  |
| IMPLEMENTS | 38 |  |
| INCLUDE | 39 |  |
| INCLUDE_ONCE | 40 |  |
| INSTANCEOF | 41 |  |
| INSTEADOF | 42 |  |
| INTERFACE | 43 |  |
| ISSET | 44 |  |
| LIST | 45 |  |
| MATCH | 46 |  |
| NAMESPACE | 47 |  |
| NEW | 48 |  |
| OR | 49 |  |
| PARENT | 77 |  |
| PRINT | 50 |  |
| PRIVATE | 51 |  |
| PROTECTED | 52 |  |
| PUBLIC | 53 |  |
| READONLY | 79 |  |
| REQUIRE | 54 |  |
| REQUIRE_ONCE | 55 |  |
| RETURN | 56 |  |
| SELF | 78 |  |
| STATIC | 57 |  |
| SWITCH | 58 |  |
| THROW | 59 |  |
| TRAIT | 60 |  |
| TRY | 61 |  |
| UNSET | 62 |  |
| USE | 63 |  |
| VAR | 64 |  |
| WHILE | 65 |  |
| XOR | 66 |  |
| YIELD | 67 |  |
| INT | 68 |  |
| FLOAT | 69 |  |
| BOOL | 70 |  |
| STRING | 71 |  |
| TRUE | 72 |  |
| FALSE | 73 |  |
| NULL | 74 |  |
| VOID | 75 |  |
| ITERABLE | 76 |  |


 

 

 



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

