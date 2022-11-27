# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [php/tests/proto/test_reserved_enum_value_lower.proto](#php_tests_proto_test_reserved_enum_value_lower-proto)
    - [NotAllowed](#lower_enum_value-NotAllowed)
  
- [Scalar Value Types](#scalar-value-types)



<a name="php_tests_proto_test_reserved_enum_value_lower-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## php/tests/proto/test_reserved_enum_value_lower.proto


 


<a name="lower_enum_value-NotAllowed"></a>

### NotAllowed


| Name | Number | Description |
| ---- | ------ | ----------- |
| abstract | 0 |  |
| and | 1 |  |
| array | 2 |  |
| as | 3 |  |
| break | 4 |  |
| callable | 5 |  |
| case | 6 |  |
| catch | 7 |  |
| class | 8 |  |
| clone | 9 |  |
| const | 10 |  |
| continue | 11 |  |
| declare | 12 |  |
| default | 13 |  |
| die | 14 |  |
| do | 15 |  |
| echo | 16 |  |
| else | 17 |  |
| elseif | 18 |  |
| empty | 19 |  |
| enddeclare | 20 |  |
| endfor | 21 |  |
| endforeach | 22 |  |
| endif | 23 |  |
| endswitch | 24 |  |
| endwhile | 25 |  |
| eval | 26 |  |
| exit | 27 |  |
| extends | 28 |  |
| final | 29 |  |
| finally | 30 |  |
| fn | 31 |  |
| for | 32 |  |
| foreach | 33 |  |
| function | 34 |  |
| global | 35 |  |
| goto | 36 |  |
| if | 37 |  |
| implements | 38 |  |
| include | 39 |  |
| include_once | 40 |  |
| instanceof | 41 |  |
| insteadof | 42 |  |
| interface | 43 |  |
| isset | 44 |  |
| list | 45 |  |
| match | 46 |  |
| namespace | 47 |  |
| new | 48 |  |
| or | 49 |  |
| parent | 77 |  |
| print | 50 |  |
| private | 51 |  |
| protected | 52 |  |
| public | 53 |  |
| readonly | 79 |  |
| require | 54 |  |
| require_once | 55 |  |
| return | 56 |  |
| self | 78 |  |
| static | 57 |  |
| switch | 58 |  |
| throw | 59 |  |
| trait | 60 |  |
| try | 61 |  |
| unset | 62 |  |
| use | 63 |  |
| var | 64 |  |
| while | 65 |  |
| xor | 66 |  |
| yield | 67 |  |
| int | 68 |  |
| float | 69 |  |
| bool | 70 |  |
| string | 71 |  |
| true | 72 |  |
| false | 73 |  |
| null | 74 |  |
| void | 75 |  |
| iterable | 76 |  |


 

 

 



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

