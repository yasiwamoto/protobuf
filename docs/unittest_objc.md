# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest_objc.proto](#objectivec_Tests_unittest_objc-proto)
    - [BoolOnlyMessage](#objc-protobuf-tests-BoolOnlyMessage)
    - [EnumTestMsg](#objc-protobuf-tests-EnumTestMsg)
    - [JustToScopeExtensions](#objc-protobuf-tests-JustToScopeExtensions)
    - [MessageWithOneBasedEnum](#objc-protobuf-tests-MessageWithOneBasedEnum)
    - [ObjCInitFoo](#objc-protobuf-tests-ObjCInitFoo)
    - [ObjCPropertyNaming](#objc-protobuf-tests-ObjCPropertyNaming)
    - [ObjCRetainedComplex](#objc-protobuf-tests-ObjCRetainedComplex)
    - [ObjCRetainedComplexRepeated](#objc-protobuf-tests-ObjCRetainedComplexRepeated)
    - [ObjCRetainedFoo](#objc-protobuf-tests-ObjCRetainedFoo)
    - [ObjCRetainedMessage](#objc-protobuf-tests-ObjCRetainedMessage)
    - [ObjCRetainedMessageRepeated](#objc-protobuf-tests-ObjCRetainedMessageRepeated)
    - [ObjCRetainedPrimitive](#objc-protobuf-tests-ObjCRetainedPrimitive)
    - [ObjCRetainedPrimitiveRepeated](#objc-protobuf-tests-ObjCRetainedPrimitiveRepeated)
    - [ObjcWeirdDefaults](#objc-protobuf-tests-ObjcWeirdDefaults)
    - [Point](#objc-protobuf-tests-Point)
    - [Point.Rect](#objc-protobuf-tests-Point-Rect)
    - [TestGeneratedComments](#objc-protobuf-tests-TestGeneratedComments)
    - [TestMessageOfMaps](#objc-protobuf-tests-TestMessageOfMaps)
    - [TestMessageOfMaps.BoolToBoolEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToBoolEntry)
    - [TestMessageOfMaps.BoolToIntEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToIntEntry)
    - [TestMessageOfMaps.BoolToMsgEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToMsgEntry)
    - [TestMessageOfMaps.BoolToStrEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToStrEntry)
    - [TestMessageOfMaps.IntToBoolEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToBoolEntry)
    - [TestMessageOfMaps.IntToIntEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToIntEntry)
    - [TestMessageOfMaps.IntToMsgEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToMsgEntry)
    - [TestMessageOfMaps.IntToStrEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToStrEntry)
    - [TestMessageOfMaps.StrToBoolEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToBoolEntry)
    - [TestMessageOfMaps.StrToIntEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToIntEntry)
    - [TestMessageOfMaps.StrToMsgEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToMsgEntry)
    - [TestMessageOfMaps.StrToStrEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToStrEntry)
    - [TestRecursiveExtension](#objc-protobuf-tests-TestRecursiveExtension)
    - [TestRecursiveMessageWithRepeatedField](#objc-protobuf-tests-TestRecursiveMessageWithRepeatedField)
    - [TestRecursiveMessageWithRepeatedField.IToIEntry](#objc-protobuf-tests-TestRecursiveMessageWithRepeatedField-IToIEntry)
    - [TestRecursiveMessageWithRepeatedField.StrToStrEntry](#objc-protobuf-tests-TestRecursiveMessageWithRepeatedField-StrToStrEntry)
    - [WKTRefereceMessage](#objc-protobuf-tests-WKTRefereceMessage)
    - [self](#objc-protobuf-tests-self)
    - [self.MutableCopy](#objc-protobuf-tests-self-MutableCopy)
    - [self.New](#objc-protobuf-tests-self-New)
    - [self.super](#objc-protobuf-tests-self-super)
  
    - [Category](#objc-protobuf-tests-Category)
    - [EnumTestMsg.MyEnum](#objc-protobuf-tests-EnumTestMsg-MyEnum)
    - [Foo](#objc-protobuf-tests-Foo)
    - [MessageWithOneBasedEnum.OneBasedEnum](#objc-protobuf-tests-MessageWithOneBasedEnum-OneBasedEnum)
    - [TestEnumObjCNameCollision](#objc-protobuf-tests-TestEnumObjCNameCollision)
    - [Time](#objc-protobuf-tests-Time)
    - [retain](#objc-protobuf-tests-retain)
    - [self.autorelease](#objc-protobuf-tests-self-autorelease)
  
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest_objc-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest_objc-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest_objc.proto



<a name="objc-protobuf-tests-BoolOnlyMessage"></a>

### BoolOnlyMessage
Message with all bools for testing things related to bool storage.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bool_field_1 | [bool](#bool) | optional |  |
| bool_field_2 | [bool](#bool) | optional |  |
| bool_field_3 | [bool](#bool) | optional |  |
| bool_field_4 | [bool](#bool) | optional |  |
| bool_field_5 | [bool](#bool) | optional |  |
| bool_field_6 | [bool](#bool) | optional |  |
| bool_field_7 | [bool](#bool) | optional |  |
| bool_field_8 | [bool](#bool) | optional |  |
| bool_field_9 | [bool](#bool) | optional |  |
| bool_field_10 | [bool](#bool) | optional |  |
| bool_field_11 | [bool](#bool) | optional |  |
| bool_field_12 | [bool](#bool) | optional |  |
| bool_field_13 | [bool](#bool) | optional |  |
| bool_field_14 | [bool](#bool) | optional |  |
| bool_field_15 | [bool](#bool) | optional |  |
| bool_field_16 | [bool](#bool) | optional |  |
| bool_field_17 | [bool](#bool) | optional |  |
| bool_field_18 | [bool](#bool) | optional |  |
| bool_field_19 | [bool](#bool) | optional |  |
| bool_field_20 | [bool](#bool) | optional |  |
| bool_field_21 | [bool](#bool) | optional |  |
| bool_field_22 | [bool](#bool) | optional |  |
| bool_field_23 | [bool](#bool) | optional |  |
| bool_field_24 | [bool](#bool) | optional |  |
| bool_field_25 | [bool](#bool) | optional |  |
| bool_field_26 | [bool](#bool) | optional |  |
| bool_field_27 | [bool](#bool) | optional |  |
| bool_field_28 | [bool](#bool) | optional |  |
| bool_field_29 | [bool](#bool) | optional |  |
| bool_field_30 | [bool](#bool) | optional |  |
| bool_field_31 | [bool](#bool) | optional |  |
| bool_field_32 | [bool](#bool) | optional |  |






<a name="objc-protobuf-tests-EnumTestMsg"></a>

### EnumTestMsg
Used to confirm negative enum values work as expected.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [EnumTestMsg.MyEnum](#objc-protobuf-tests-EnumTestMsg-MyEnum) | optional |  |
| bar | [EnumTestMsg.MyEnum](#objc-protobuf-tests-EnumTestMsg-MyEnum) | optional |  Default: ONE |
| baz | [EnumTestMsg.MyEnum](#objc-protobuf-tests-EnumTestMsg-MyEnum) | optional |  Default: NEG_ONE |
| mumble | [EnumTestMsg.MyEnum](#objc-protobuf-tests-EnumTestMsg-MyEnum) | repeated |  |






<a name="objc-protobuf-tests-JustToScopeExtensions"></a>

### JustToScopeExtensions





| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| new_val_lower_complex | string | ObjCRetainedFoo | 2011 |  |
| new_Val_upper_complex | string | ObjCRetainedFoo | 2012 |  |
| newvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 2013 |  |
| newValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 2014 |  |
| new_val_lower_primitive | int32 | ObjCRetainedFoo | 2015 |  |
| new_Val_upper_primitive | int32 | ObjCRetainedFoo | 2016 |  |
| newvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 2017 |  |
| newValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 2018 |  |
| new_val_lower_message | self | ObjCRetainedFoo | 2019 |  |
| new_Val_upper_message | self | ObjCRetainedFoo | 2020 |  |
| newvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 2021 |  |
| newValue_upper_no_underscore_message | self | ObjCRetainedFoo | 2022 |  |
| new_val_lower_enum | Foo | ObjCRetainedFoo | 2023 |  |
| new_Val_upper_enum | Foo | ObjCRetainedFoo | 2024 |  |
| newvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 2025 |  |
| newValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 2026 |  |
| new_val_lower_complex_repeated | string | ObjCRetainedFoo | 2111 |  |
| new_Val_upper_complex_repeated | string | ObjCRetainedFoo | 2112 |  |
| newvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2113 |  |
| newValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2114 |  |
| new_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 2115 |  |
| new_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 2116 |  |
| newvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2117 |  |
| newValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2118 |  |
| new_val_lower_message_repeated | self | ObjCRetainedFoo | 2119 |  |
| new_Val_upper_message_repeated | self | ObjCRetainedFoo | 2120 |  |
| newvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 2121 |  |
| newValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 2122 |  |
| new_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 2123 |  |
| new_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 2124 |  |
| newvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2125 |  |
| newValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2126 |  |
| alloc_val_lower_complex | string | ObjCRetainedFoo | 2211 |  |
| alloc_Val_upper_complex | string | ObjCRetainedFoo | 2212 |  |
| allocvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 2213 |  |
| allocValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 2214 |  |
| alloc_val_lower_primitive | int32 | ObjCRetainedFoo | 2215 |  |
| alloc_Val_upper_primitive | int32 | ObjCRetainedFoo | 2216 |  |
| allocvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 2217 |  |
| allocValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 2218 |  |
| alloc_val_lower_message | self | ObjCRetainedFoo | 2219 |  |
| alloc_Val_upper_message | self | ObjCRetainedFoo | 2220 |  |
| allocvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 2221 |  |
| allocValue_upper_no_underscore_message | self | ObjCRetainedFoo | 2222 |  |
| alloc_val_lower_enum | Foo | ObjCRetainedFoo | 2223 |  |
| alloc_Val_upper_enum | Foo | ObjCRetainedFoo | 2224 |  |
| allocvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 2225 |  |
| allocValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 2226 |  |
| alloc_val_lower_complex_repeated | string | ObjCRetainedFoo | 2311 |  |
| alloc_Val_upper_complex_repeated | string | ObjCRetainedFoo | 2312 |  |
| allocvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2313 |  |
| allocValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2314 |  |
| alloc_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 2315 |  |
| alloc_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 2316 |  |
| allocvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2317 |  |
| allocValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2318 |  |
| alloc_val_lower_message_repeated | self | ObjCRetainedFoo | 2319 |  |
| alloc_Val_upper_message_repeated | self | ObjCRetainedFoo | 2320 |  |
| allocvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 2321 |  |
| allocValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 2322 |  |
| alloc_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 2323 |  |
| alloc_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 2324 |  |
| allocvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2325 |  |
| allocValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2326 |  |
| copy_val_lower_complex | string | ObjCRetainedFoo | 2411 |  |
| copy_Val_upper_complex | string | ObjCRetainedFoo | 2412 |  |
| copyvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 2413 |  |
| copyValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 2414 |  |
| copy_val_lower_primitive | int32 | ObjCRetainedFoo | 2415 |  |
| copy_Val_upper_primitive | int32 | ObjCRetainedFoo | 2416 |  |
| copyvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 2417 |  |
| copyValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 2418 |  |
| copy_val_lower_message | self | ObjCRetainedFoo | 2419 |  |
| copy_Val_upper_message | self | ObjCRetainedFoo | 2420 |  |
| copyvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 2421 |  |
| copyValue_upper_no_underscore_message | self | ObjCRetainedFoo | 2422 |  |
| copy_val_lower_enum | Foo | ObjCRetainedFoo | 2423 |  |
| copy_Val_upper_enum | Foo | ObjCRetainedFoo | 2424 |  |
| copyvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 2425 |  |
| copyValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 2426 |  |
| copy_val_lower_complex_repeated | string | ObjCRetainedFoo | 2511 |  |
| copy_Val_upper_complex_repeated | string | ObjCRetainedFoo | 2512 |  |
| copyvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2513 |  |
| copyValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2514 |  |
| copy_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 2515 |  |
| copy_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 2516 |  |
| copyvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2517 |  |
| copyValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2518 |  |
| copy_val_lower_message_repeated | self | ObjCRetainedFoo | 2519 |  |
| copy_Val_upper_message_repeated | self | ObjCRetainedFoo | 2520 |  |
| copyvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 2521 |  |
| copyValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 2522 |  |
| copy_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 2523 |  |
| copy_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 2524 |  |
| copyvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2525 |  |
| copyValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2526 |  |
| mutableCopy_val_lower_complex | string | ObjCRetainedFoo | 2611 |  |
| mutableCopy_Val_upper_complex | string | ObjCRetainedFoo | 2612 |  |
| mutableCopyvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 2613 |  |
| mutableCopyValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 2614 |  |
| mutableCopy_val_lower_primitive | int32 | ObjCRetainedFoo | 2615 |  |
| mutableCopy_Val_upper_primitive | int32 | ObjCRetainedFoo | 2616 |  |
| mutableCopyvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 2617 |  |
| mutableCopyValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 2618 |  |
| mutableCopy_val_lower_message | self | ObjCRetainedFoo | 2619 |  |
| mutableCopy_Val_upper_message | self | ObjCRetainedFoo | 2620 |  |
| mutableCopyvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 2621 |  |
| mutableCopyValue_upper_no_underscore_message | self | ObjCRetainedFoo | 2622 |  |
| mutableCopy_val_lower_enum | Foo | ObjCRetainedFoo | 2623 |  |
| mutableCopy_Val_upper_enum | Foo | ObjCRetainedFoo | 2624 |  |
| mutableCopyvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 2625 |  |
| mutableCopyValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 2626 |  |
| mutableCopy_val_lower_complex_repeated | string | ObjCRetainedFoo | 2711 |  |
| mutableCopy_Val_upper_complex_repeated | string | ObjCRetainedFoo | 2712 |  |
| mutableCopyvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2713 |  |
| mutableCopyValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 2714 |  |
| mutableCopy_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 2715 |  |
| mutableCopy_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 2716 |  |
| mutableCopyvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2717 |  |
| mutableCopyValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 2718 |  |
| mutableCopy_val_lower_message_repeated | self | ObjCRetainedFoo | 2719 |  |
| mutableCopy_Val_upper_message_repeated | self | ObjCRetainedFoo | 2720 |  |
| mutableCopyvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 2721 |  |
| mutableCopyValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 2722 |  |
| mutableCopy_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 2723 |  |
| mutableCopy_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 2724 |  |
| mutableCopyvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2725 |  |
| mutableCopyValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 2726 |  |




<a name="objc-protobuf-tests-MessageWithOneBasedEnum"></a>

### MessageWithOneBasedEnum
Test case for https://github.com/protocolbuffers/protobuf/issues/1453
Message with no explicit defaults, but a non zero default for an enum.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| enum_field | [MessageWithOneBasedEnum.OneBasedEnum](#objc-protobuf-tests-MessageWithOneBasedEnum-OneBasedEnum) | optional |  |






<a name="objc-protobuf-tests-ObjCInitFoo"></a>

### ObjCInitFoo
Test handing of fields that start with init*.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| init_val | [string](#string) | optional |  |
| init_size | [int32](#int32) | optional |  |
| init_self | [self](#objc-protobuf-tests-self) | optional |  |
| init_vals | [string](#string) | repeated |  |
| init_sizes | [int32](#int32) | repeated |  |
| init_selfs | [self](#objc-protobuf-tests-self) | repeated |  |






<a name="objc-protobuf-tests-ObjCPropertyNaming"></a>

### ObjCPropertyNaming



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| url | [string](#string) | optional | Test that the properties properly get things all caps. |
| thumbnail_url | [string](#string) | optional |  |
| url_foo | [string](#string) | optional |  |
| some_url_blah | [string](#string) | optional |  |
| http | [string](#string) | optional |  |
| https | [string](#string) | optional |  |
| urls | [string](#string) | repeated | This one doesn&#39;t. |






<a name="objc-protobuf-tests-ObjCRetainedComplex"></a>

### ObjCRetainedComplex
Test handling of fields that are the retained names.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new | [string](#string) | optional |  |
| alloc | [string](#string) | optional |  |
| copy | [string](#string) | optional |  |
| mutableCopy | [string](#string) | optional |  |






<a name="objc-protobuf-tests-ObjCRetainedComplexRepeated"></a>

### ObjCRetainedComplexRepeated



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new | [string](#string) | repeated |  |
| alloc | [string](#string) | repeated |  |
| copy | [string](#string) | repeated |  |
| mutableCopy | [string](#string) | repeated |  |






<a name="objc-protobuf-tests-ObjCRetainedFoo"></a>

### ObjCRetainedFoo
Test handling of fields that start with retained names.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new_val_lower_complex | [string](#string) | optional |  |
| new_Val_upper_complex | [string](#string) | optional |  |
| newvalue_lower_no_underscore_complex | [string](#string) | optional |  |
| newValue_upper_no_underscore_complex | [string](#string) | optional |  |
| new_val_lower_primitive | [int32](#int32) | optional |  |
| new_Val_upper_primitive | [int32](#int32) | optional |  |
| newvalue_lower_no_underscore_primitive | [int32](#int32) | optional |  |
| newValue_upper_no_underscore_primitive | [int32](#int32) | optional |  |
| new_val_lower_message | [self](#objc-protobuf-tests-self) | optional |  |
| new_Val_upper_message | [self](#objc-protobuf-tests-self) | optional |  |
| newvalue_lower_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| newValue_upper_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| new_val_lower_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| new_Val_upper_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| newvalue_lower_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| newValue_upper_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| new_val_lower_complex_repeated | [string](#string) | repeated |  |
| new_Val_upper_complex_repeated | [string](#string) | repeated |  |
| newvalue_lower_no_underscore_complex_repeated | [string](#string) | repeated |  |
| newValue_upper_no_underscore_complex_repeated | [string](#string) | repeated |  |
| new_val_lower_primitive_repeated | [int32](#int32) | repeated |  |
| new_Val_upper_primitive_repeated | [int32](#int32) | repeated |  |
| newvalue_lower_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| newValue_upper_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| new_val_lower_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| new_Val_upper_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| newvalue_lower_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| newValue_upper_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| new_val_lower_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| new_Val_upper_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| newvalue_lower_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| newValue_upper_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| alloc_val_lower_complex | [string](#string) | optional |  |
| alloc_Val_upper_complex | [string](#string) | optional |  |
| allocvalue_lower_no_underscore_complex | [string](#string) | optional |  |
| allocValue_upper_no_underscore_complex | [string](#string) | optional |  |
| alloc_val_lower_primitive | [int32](#int32) | optional |  |
| alloc_Val_upper_primitive | [int32](#int32) | optional |  |
| allocvalue_lower_no_underscore_primitive | [int32](#int32) | optional |  |
| allocValue_upper_no_underscore_primitive | [int32](#int32) | optional |  |
| alloc_val_lower_message | [self](#objc-protobuf-tests-self) | optional |  |
| alloc_Val_upper_message | [self](#objc-protobuf-tests-self) | optional |  |
| allocvalue_lower_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| allocValue_upper_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| alloc_val_lower_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| alloc_Val_upper_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| allocvalue_lower_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| allocValue_upper_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| alloc_val_lower_complex_repeated | [string](#string) | repeated |  |
| alloc_Val_upper_complex_repeated | [string](#string) | repeated |  |
| allocvalue_lower_no_underscore_complex_repeated | [string](#string) | repeated |  |
| allocValue_upper_no_underscore_complex_repeated | [string](#string) | repeated |  |
| alloc_val_lower_primitive_repeated | [int32](#int32) | repeated |  |
| alloc_Val_upper_primitive_repeated | [int32](#int32) | repeated |  |
| allocvalue_lower_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| allocValue_upper_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| alloc_val_lower_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| alloc_Val_upper_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| allocvalue_lower_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| allocValue_upper_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| alloc_val_lower_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| alloc_Val_upper_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| allocvalue_lower_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| allocValue_upper_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| copy_val_lower_complex | [string](#string) | optional |  |
| copy_Val_upper_complex | [string](#string) | optional |  |
| copyvalue_lower_no_underscore_complex | [string](#string) | optional |  |
| copyValue_upper_no_underscore_complex | [string](#string) | optional |  |
| copy_val_lower_primitive | [int32](#int32) | optional |  |
| copy_Val_upper_primitive | [int32](#int32) | optional |  |
| copyvalue_lower_no_underscore_primitive | [int32](#int32) | optional |  |
| copyValue_upper_no_underscore_primitive | [int32](#int32) | optional |  |
| copy_val_lower_message | [self](#objc-protobuf-tests-self) | optional |  |
| copy_Val_upper_message | [self](#objc-protobuf-tests-self) | optional |  |
| copyvalue_lower_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| copyValue_upper_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| copy_val_lower_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| copy_Val_upper_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| copyvalue_lower_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| copyValue_upper_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| copy_val_lower_complex_repeated | [string](#string) | repeated |  |
| copy_Val_upper_complex_repeated | [string](#string) | repeated |  |
| copyvalue_lower_no_underscore_complex_repeated | [string](#string) | repeated |  |
| copyValue_upper_no_underscore_complex_repeated | [string](#string) | repeated |  |
| copy_val_lower_primitive_repeated | [int32](#int32) | repeated |  |
| copy_Val_upper_primitive_repeated | [int32](#int32) | repeated |  |
| copyvalue_lower_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| copyValue_upper_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| copy_val_lower_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| copy_Val_upper_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| copyvalue_lower_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| copyValue_upper_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| copy_val_lower_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| copy_Val_upper_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| copyvalue_lower_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| copyValue_upper_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| mutableCopy_val_lower_complex | [string](#string) | optional |  |
| mutableCopy_Val_upper_complex | [string](#string) | optional |  |
| mutableCopyvalue_lower_no_underscore_complex | [string](#string) | optional |  |
| mutableCopyValue_upper_no_underscore_complex | [string](#string) | optional |  |
| mutableCopy_val_lower_primitive | [int32](#int32) | optional |  |
| mutableCopy_Val_upper_primitive | [int32](#int32) | optional |  |
| mutableCopyvalue_lower_no_underscore_primitive | [int32](#int32) | optional |  |
| mutableCopyValue_upper_no_underscore_primitive | [int32](#int32) | optional |  |
| mutableCopy_val_lower_message | [self](#objc-protobuf-tests-self) | optional |  |
| mutableCopy_Val_upper_message | [self](#objc-protobuf-tests-self) | optional |  |
| mutableCopyvalue_lower_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| mutableCopyValue_upper_no_underscore_message | [self](#objc-protobuf-tests-self) | optional |  |
| mutableCopy_val_lower_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| mutableCopy_Val_upper_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| mutableCopyvalue_lower_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| mutableCopyValue_upper_no_underscore_enum | [Foo](#objc-protobuf-tests-Foo) | optional |  |
| mutableCopy_val_lower_complex_repeated | [string](#string) | repeated |  |
| mutableCopy_Val_upper_complex_repeated | [string](#string) | repeated |  |
| mutableCopyvalue_lower_no_underscore_complex_repeated | [string](#string) | repeated |  |
| mutableCopyValue_upper_no_underscore_complex_repeated | [string](#string) | repeated |  |
| mutableCopy_val_lower_primitive_repeated | [int32](#int32) | repeated |  |
| mutableCopy_Val_upper_primitive_repeated | [int32](#int32) | repeated |  |
| mutableCopyvalue_lower_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| mutableCopyValue_upper_no_underscore_primitive_repeated | [int32](#int32) | repeated |  |
| mutableCopy_val_lower_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| mutableCopy_Val_upper_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| mutableCopyvalue_lower_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| mutableCopyValue_upper_no_underscore_message_repeated | [self](#objc-protobuf-tests-self) | repeated |  |
| mutableCopy_val_lower_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| mutableCopy_Val_upper_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| mutableCopyvalue_lower_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |
| mutableCopyValue_upper_no_underscore_enum_repeated | [Foo](#objc-protobuf-tests-Foo) | repeated |  |






<a name="objc-protobuf-tests-ObjCRetainedMessage"></a>

### ObjCRetainedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new | [self](#objc-protobuf-tests-self) | optional |  |
| alloc | [self](#objc-protobuf-tests-self) | optional |  |
| copy | [self](#objc-protobuf-tests-self) | optional |  |
| mutableCopy | [self](#objc-protobuf-tests-self) | optional |  |






<a name="objc-protobuf-tests-ObjCRetainedMessageRepeated"></a>

### ObjCRetainedMessageRepeated



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new | [self](#objc-protobuf-tests-self) | repeated |  |
| alloc | [self](#objc-protobuf-tests-self) | repeated |  |
| copy | [self](#objc-protobuf-tests-self) | repeated |  |
| mutableCopy | [self](#objc-protobuf-tests-self) | repeated |  |






<a name="objc-protobuf-tests-ObjCRetainedPrimitive"></a>

### ObjCRetainedPrimitive



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new | [int32](#int32) | optional |  |
| alloc | [int32](#int32) | optional |  |
| copy | [int32](#int32) | optional |  |
| mutableCopy | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-ObjCRetainedPrimitiveRepeated"></a>

### ObjCRetainedPrimitiveRepeated



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| new | [int32](#int32) | repeated |  |
| alloc | [int32](#int32) | repeated |  |
| copy | [int32](#int32) | repeated |  |
| mutableCopy | [int32](#int32) | repeated |  |






<a name="objc-protobuf-tests-ObjcWeirdDefaults"></a>

### ObjcWeirdDefaults
Test some weird defaults that we see in protos.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [string](#string) | optional | Set default values that match the protocol buffer defined defaults to confirm hasDefault and the default values are set correctly. |
| bar | [bytes](#bytes) | optional |  |






<a name="objc-protobuf-tests-Point"></a>

### Point
Test Handling some MacTypes






<a name="objc-protobuf-tests-Point-Rect"></a>

### Point.Rect



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| TimeValue | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestGeneratedComments"></a>

### TestGeneratedComments
Used to check that Headerdocs and appledoc work correctly. If these comments
are not handled correctly, Xcode will fail to build the tests.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| string_field | [string](#string) | optional | This is a string that could contain stuff like mime types as image/* or */plain. Maybe twitter usernames like @protobuf, @google or @something. |






<a name="objc-protobuf-tests-TestMessageOfMaps"></a>

### TestMessageOfMaps
Message with a few types of maps to cover the different custom flows
in the runtime.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| str_to_str | [TestMessageOfMaps.StrToStrEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToStrEntry) | repeated |  |
| str_to_int | [TestMessageOfMaps.StrToIntEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToIntEntry) | repeated |  |
| int_to_str | [TestMessageOfMaps.IntToStrEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToStrEntry) | repeated |  |
| int_to_int | [TestMessageOfMaps.IntToIntEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToIntEntry) | repeated |  |
| str_to_bool | [TestMessageOfMaps.StrToBoolEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToBoolEntry) | repeated |  |
| bool_to_str | [TestMessageOfMaps.BoolToStrEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToStrEntry) | repeated |  |
| bool_to_bool | [TestMessageOfMaps.BoolToBoolEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToBoolEntry) | repeated |  |
| int_to_bool | [TestMessageOfMaps.IntToBoolEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToBoolEntry) | repeated |  |
| bool_to_int | [TestMessageOfMaps.BoolToIntEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToIntEntry) | repeated |  |
| str_to_msg | [TestMessageOfMaps.StrToMsgEntry](#objc-protobuf-tests-TestMessageOfMaps-StrToMsgEntry) | repeated |  |
| int_to_msg | [TestMessageOfMaps.IntToMsgEntry](#objc-protobuf-tests-TestMessageOfMaps-IntToMsgEntry) | repeated |  |
| bool_to_msg | [TestMessageOfMaps.BoolToMsgEntry](#objc-protobuf-tests-TestMessageOfMaps-BoolToMsgEntry) | repeated |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-BoolToBoolEntry"></a>

### TestMessageOfMaps.BoolToBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-BoolToIntEntry"></a>

### TestMessageOfMaps.BoolToIntEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-BoolToMsgEntry"></a>

### TestMessageOfMaps.BoolToMsgEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-BoolToStrEntry"></a>

### TestMessageOfMaps.BoolToStrEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-IntToBoolEntry"></a>

### TestMessageOfMaps.IntToBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-IntToIntEntry"></a>

### TestMessageOfMaps.IntToIntEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-IntToMsgEntry"></a>

### TestMessageOfMaps.IntToMsgEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-IntToStrEntry"></a>

### TestMessageOfMaps.IntToStrEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-StrToBoolEntry"></a>

### TestMessageOfMaps.StrToBoolEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-StrToIntEntry"></a>

### TestMessageOfMaps.StrToIntEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-StrToMsgEntry"></a>

### TestMessageOfMaps.StrToMsgEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestMessageOfMaps-StrToStrEntry"></a>

### TestMessageOfMaps.StrToStrEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestRecursiveExtension"></a>

### TestRecursiveExtension
Recursive message and extension to for testing autocreators at different
depths.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| recursive_sub_message | [TestRecursiveExtension](#objc-protobuf-tests-TestRecursiveExtension) | optional |  |
| repeated_value | [int32](#int32) | repeated |  |






<a name="objc-protobuf-tests-TestRecursiveMessageWithRepeatedField"></a>

### TestRecursiveMessageWithRepeatedField
Recursive message to for testing autocreators at different depths.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [TestRecursiveMessageWithRepeatedField](#objc-protobuf-tests-TestRecursiveMessageWithRepeatedField) | optional |  |
| i | [int32](#int32) | repeated |  |
| str | [string](#string) | repeated |  |
| i_to_i | [TestRecursiveMessageWithRepeatedField.IToIEntry](#objc-protobuf-tests-TestRecursiveMessageWithRepeatedField-IToIEntry) | repeated |  |
| str_to_str | [TestRecursiveMessageWithRepeatedField.StrToStrEntry](#objc-protobuf-tests-TestRecursiveMessageWithRepeatedField-StrToStrEntry) | repeated |  |






<a name="objc-protobuf-tests-TestRecursiveMessageWithRepeatedField-IToIEntry"></a>

### TestRecursiveMessageWithRepeatedField.IToIEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestRecursiveMessageWithRepeatedField-StrToStrEntry"></a>

### TestRecursiveMessageWithRepeatedField.StrToStrEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="objc-protobuf-tests-WKTRefereceMessage"></a>

### WKTRefereceMessage
Reference to a WKT to test (via generated code inspection), the handling
of #imports.  Within the WKTs, references to each other are just path
based imports, but when reference from another proto file, they should be
conditional to support the framework import style.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| an_any | [google.protobuf.Any](#google-protobuf-Any) | optional |  |






<a name="objc-protobuf-tests-self"></a>

### self



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [bool](#bool) | optional | Singular Objective C Keywords |
| _cmd | [bool](#bool) | optional |  |
| in | [bool](#bool) | optional | super is used as submessage above |
| out | [bool](#bool) | optional |  |
| inout | [bool](#bool) | optional |  |
| bycopy | [bool](#bool) | optional |  |
| byref | [bool](#bool) | optional |  |
| oneway | [bool](#bool) | optional |  |
| self | [bool](#bool) | optional |  |
| instancetype | [bool](#bool) | optional |  |
| nullable | [bool](#bool) | optional |  |
| nonnull | [bool](#bool) | optional |  |
| nil | [bool](#bool) | optional |  |
| YES | [bool](#bool) | optional | Nil and nil can&#39;t be in the same message |
| NO | [bool](#bool) | optional |  |
| weak | [bool](#bool) | optional |  |
| case | [bool](#bool) | optional | Some C/C&#43;&#43; Keywords |
| if | [bool](#bool) | optional |  |
| and_eq | [bool](#bool) | optional |  |
| public | [bool](#bool) | optional |  |
| private | [bool](#bool) | optional |  |
| typename | [bool](#bool) | optional |  |
| static_cast | [bool](#bool) | optional |  |
| typeof | [bool](#bool) | optional |  |
| restrict | [bool](#bool) | optional |  |
| NULL | [bool](#bool) | optional |  |
| dealloc | [bool](#bool) | optional | Some NSObject Methods |
| isProxy | [bool](#bool) | optional |  |
| copy | [bool](#bool) | optional |  |
| description | [bool](#bool) | optional |  |
| zone | [bool](#bool) | optional |  |
| className | [bool](#bool) | optional |  |
| __retain_OA | [bool](#bool) | optional |  |
| CAMLType | [bool](#bool) | optional |  |
| isNSDictionary__ | [bool](#bool) | optional |  |
| accessibilityLabel | [bool](#bool) | optional |  |
| assign | [bool](#bool) | optional | Some Objc &#34;keywords&#34; that we shouldn&#39;t have to worry about because they can only appear in specialized areas. |
| getter | [bool](#bool) | optional |  |
| setter | [bool](#bool) | optional |  |
| atomic | [bool](#bool) | optional |  |
| nonatomic | [bool](#bool) | optional |  |
| strong | [bool](#bool) | optional |  |
| null_resettable | [bool](#bool) | optional |  |
| readonly | [bool](#bool) | optional |  |
| clear | [bool](#bool) | optional | Some GPBMessage methods |
| data | [bool](#bool) | optional |  |
| descriptor | [bool](#bool) | optional |  |
| delimitedData | [bool](#bool) | optional |  |
| Fixed | [bool](#bool) | optional | Some MacTypes |
| Point | [bool](#bool) | optional |  |
| FixedPoint | [bool](#bool) | optional |  |
| Style | [bool](#bool) | optional |  |
| _Generic | [bool](#bool) | optional | C/C&#43;&#43; reserved identifiers |
| __block | [bool](#bool) | optional |  |
| SubEnum | [self.autorelease](#objc-protobuf-tests-self-autorelease) | optional | Try a keyword as a type |
| new | [self.New](#objc-protobuf-tests-self-New) | optional |  |
| mutablecopy | [self.MutableCopy](#objc-protobuf-tests-self-MutableCopy) | optional |  |






<a name="objc-protobuf-tests-self-MutableCopy"></a>

### self.MutableCopy



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| extensionRegistry | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-self-New"></a>

### self.New



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| copy | [string](#string) | optional |  |






<a name="objc-protobuf-tests-self-super"></a>

### self.super



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| description | [int32](#int32) | optional |  |





 


<a name="objc-protobuf-tests-Category"></a>

### Category
EnumValueShortName: The enum name gets a prefix.

| Name | Number | Description |
| ---- | ------ | ----------- |
| RED | 1 |  |
| BLUE | 2 |  |



<a name="objc-protobuf-tests-EnumTestMsg-MyEnum"></a>

### EnumTestMsg.MyEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |
| TWO | 2 |  |
| NEG_ONE | -1 |  |
| NEG_TWO | -2 |  |



<a name="objc-protobuf-tests-Foo"></a>

### Foo
EnumValueShortName: The short names shouldn&#39;t get suffixes/prefixes.

| Name | Number | Description |
| ---- | ------ | ----------- |
| SERIALIZED_SIZE | 1 |  |
| SIZE | 2 |  |
| OTHER | 3 |  |



<a name="objc-protobuf-tests-MessageWithOneBasedEnum-OneBasedEnum"></a>

### MessageWithOneBasedEnum.OneBasedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ONE | 1 |  |
| TWO | 2 |  |



<a name="objc-protobuf-tests-TestEnumObjCNameCollision"></a>

### TestEnumObjCNameCollision
This is in part a compile test, it ensures that when aliases end up with
the same ObjC name, we drop them to avoid the duplication names. There
is a test to ensure the descriptors are still generated to support
reflection and TextFormat.

| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 1 |  |
| foo | 1 |  |
| BAR | 2 |  |
| mumble | 2 |  |
| MUMBLE | 2 |  |



<a name="objc-protobuf-tests-Time"></a>

### Time
EnumValueShortName: Twist case, full name gets PB, but the short names
should still end up correct.

| Name | Number | Description |
| ---- | ------ | ----------- |
| BASE | 1 |  |
| RECORD | 2 |  |
| SOMETHING_ELSE | 3 |  |



<a name="objc-protobuf-tests-retain"></a>

### retain


| Name | Number | Description |
| ---- | ------ | ----------- |
| count | 4 |  |
| initialized | 5 |  |
| serializedSize | 6 |  |



<a name="objc-protobuf-tests-self-autorelease"></a>

### self.autorelease


| Name | Number | Description |
| ---- | ------ | ----------- |
| retain | 1 |  |
| release | 2 |  |
| retainCount | 3 |  |


 


<a name="objectivec_Tests_unittest_objc-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| allocValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 1214 |  |
| allocValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1314 |  |
| allocValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 1226 |  |
| allocValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1326 |  |
| allocValue_upper_no_underscore_message | self | ObjCRetainedFoo | 1222 |  |
| allocValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 1322 |  |
| allocValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 1218 |  |
| allocValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1318 |  |
| alloc_Val_upper_complex | string | ObjCRetainedFoo | 1212 |  |
| alloc_Val_upper_complex_repeated | string | ObjCRetainedFoo | 1312 |  |
| alloc_Val_upper_enum | Foo | ObjCRetainedFoo | 1224 |  |
| alloc_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 1324 |  |
| alloc_Val_upper_message | self | ObjCRetainedFoo | 1220 |  |
| alloc_Val_upper_message_repeated | self | ObjCRetainedFoo | 1320 |  |
| alloc_Val_upper_primitive | int32 | ObjCRetainedFoo | 1216 |  |
| alloc_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 1316 |  |
| alloc_val_lower_complex | string | ObjCRetainedFoo | 1211 |  |
| alloc_val_lower_complex_repeated | string | ObjCRetainedFoo | 1311 |  |
| alloc_val_lower_enum | Foo | ObjCRetainedFoo | 1223 |  |
| alloc_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 1323 |  |
| alloc_val_lower_message | self | ObjCRetainedFoo | 1219 |  |
| alloc_val_lower_message_repeated | self | ObjCRetainedFoo | 1319 |  |
| alloc_val_lower_primitive | int32 | ObjCRetainedFoo | 1215 |  |
| alloc_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 1315 |  |
| allocvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 1213 |  |
| allocvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1313 |  |
| allocvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 1225 |  |
| allocvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1325 |  |
| allocvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 1221 |  |
| allocvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 1321 |  |
| allocvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 1217 |  |
| allocvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1317 |  |
| copyValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 1414 |  |
| copyValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1514 |  |
| copyValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 1426 |  |
| copyValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1526 |  |
| copyValue_upper_no_underscore_message | self | ObjCRetainedFoo | 1422 |  |
| copyValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 1522 |  |
| copyValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 1418 |  |
| copyValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1518 |  |
| copy_Val_upper_complex | string | ObjCRetainedFoo | 1412 |  |
| copy_Val_upper_complex_repeated | string | ObjCRetainedFoo | 1512 |  |
| copy_Val_upper_enum | Foo | ObjCRetainedFoo | 1424 |  |
| copy_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 1524 |  |
| copy_Val_upper_message | self | ObjCRetainedFoo | 1420 |  |
| copy_Val_upper_message_repeated | self | ObjCRetainedFoo | 1520 |  |
| copy_Val_upper_primitive | int32 | ObjCRetainedFoo | 1416 |  |
| copy_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 1516 |  |
| copy_val_lower_complex | string | ObjCRetainedFoo | 1411 |  |
| copy_val_lower_complex_repeated | string | ObjCRetainedFoo | 1511 |  |
| copy_val_lower_enum | Foo | ObjCRetainedFoo | 1423 |  |
| copy_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 1523 |  |
| copy_val_lower_message | self | ObjCRetainedFoo | 1419 |  |
| copy_val_lower_message_repeated | self | ObjCRetainedFoo | 1519 |  |
| copy_val_lower_primitive | int32 | ObjCRetainedFoo | 1415 |  |
| copy_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 1515 |  |
| copyvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 1413 |  |
| copyvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1513 |  |
| copyvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 1425 |  |
| copyvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1525 |  |
| copyvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 1421 |  |
| copyvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 1521 |  |
| copyvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 1417 |  |
| copyvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1517 |  |
| mutableCopyValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 1614 |  |
| mutableCopyValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1714 |  |
| mutableCopyValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 1626 |  |
| mutableCopyValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1726 |  |
| mutableCopyValue_upper_no_underscore_message | self | ObjCRetainedFoo | 1622 |  |
| mutableCopyValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 1722 |  |
| mutableCopyValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 1618 |  |
| mutableCopyValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1718 |  |
| mutableCopy_Val_upper_complex | string | ObjCRetainedFoo | 1612 |  |
| mutableCopy_Val_upper_complex_repeated | string | ObjCRetainedFoo | 1712 |  |
| mutableCopy_Val_upper_enum | Foo | ObjCRetainedFoo | 1624 |  |
| mutableCopy_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 1724 |  |
| mutableCopy_Val_upper_message | self | ObjCRetainedFoo | 1620 |  |
| mutableCopy_Val_upper_message_repeated | self | ObjCRetainedFoo | 1720 |  |
| mutableCopy_Val_upper_primitive | int32 | ObjCRetainedFoo | 1616 |  |
| mutableCopy_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 1716 |  |
| mutableCopy_val_lower_complex | string | ObjCRetainedFoo | 1611 |  |
| mutableCopy_val_lower_complex_repeated | string | ObjCRetainedFoo | 1711 |  |
| mutableCopy_val_lower_enum | Foo | ObjCRetainedFoo | 1623 |  |
| mutableCopy_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 1723 |  |
| mutableCopy_val_lower_message | self | ObjCRetainedFoo | 1619 |  |
| mutableCopy_val_lower_message_repeated | self | ObjCRetainedFoo | 1719 |  |
| mutableCopy_val_lower_primitive | int32 | ObjCRetainedFoo | 1615 |  |
| mutableCopy_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 1715 |  |
| mutableCopyvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 1613 |  |
| mutableCopyvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1713 |  |
| mutableCopyvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 1625 |  |
| mutableCopyvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1725 |  |
| mutableCopyvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 1621 |  |
| mutableCopyvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 1721 |  |
| mutableCopyvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 1617 |  |
| mutableCopyvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1717 |  |
| newValue_upper_no_underscore_complex | string | ObjCRetainedFoo | 1014 |  |
| newValue_upper_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1114 |  |
| newValue_upper_no_underscore_enum | Foo | ObjCRetainedFoo | 1026 |  |
| newValue_upper_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1126 |  |
| newValue_upper_no_underscore_message | self | ObjCRetainedFoo | 1022 |  |
| newValue_upper_no_underscore_message_repeated | self | ObjCRetainedFoo | 1122 |  |
| newValue_upper_no_underscore_primitive | int32 | ObjCRetainedFoo | 1018 |  |
| newValue_upper_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1118 |  |
| new_Val_upper_complex | string | ObjCRetainedFoo | 1012 |  |
| new_Val_upper_complex_repeated | string | ObjCRetainedFoo | 1112 |  |
| new_Val_upper_enum | Foo | ObjCRetainedFoo | 1024 |  |
| new_Val_upper_enum_repeated | Foo | ObjCRetainedFoo | 1124 |  |
| new_Val_upper_message | self | ObjCRetainedFoo | 1020 |  |
| new_Val_upper_message_repeated | self | ObjCRetainedFoo | 1120 |  |
| new_Val_upper_primitive | int32 | ObjCRetainedFoo | 1016 |  |
| new_Val_upper_primitive_repeated | int32 | ObjCRetainedFoo | 1116 |  |
| new_val_lower_complex | string | ObjCRetainedFoo | 1011 |  |
| new_val_lower_complex_repeated | string | ObjCRetainedFoo | 1111 |  |
| new_val_lower_enum | Foo | ObjCRetainedFoo | 1023 |  |
| new_val_lower_enum_repeated | Foo | ObjCRetainedFoo | 1123 |  |
| new_val_lower_message | self | ObjCRetainedFoo | 1019 |  |
| new_val_lower_message_repeated | self | ObjCRetainedFoo | 1119 |  |
| new_val_lower_primitive | int32 | ObjCRetainedFoo | 1015 |  |
| new_val_lower_primitive_repeated | int32 | ObjCRetainedFoo | 1115 |  |
| newvalue_lower_no_underscore_complex | string | ObjCRetainedFoo | 1013 |  |
| newvalue_lower_no_underscore_complex_repeated | string | ObjCRetainedFoo | 1113 |  |
| newvalue_lower_no_underscore_enum | Foo | ObjCRetainedFoo | 1025 |  |
| newvalue_lower_no_underscore_enum_repeated | Foo | ObjCRetainedFoo | 1125 |  |
| newvalue_lower_no_underscore_message | self | ObjCRetainedFoo | 1021 |  |
| newvalue_lower_no_underscore_message_repeated | self | ObjCRetainedFoo | 1121 |  |
| newvalue_lower_no_underscore_primitive | int32 | ObjCRetainedFoo | 1017 |  |
| newvalue_lower_no_underscore_primitive_repeated | int32 | ObjCRetainedFoo | 1117 |  |
| recursive_extension | TestAllExtensions | TestAllExtensions | 86 |  |
| recursive_message_extension | TestRecursiveExtension | TestRecursiveExtension | 1000 |  |
| byref | sint32 | self | 3004 |  |
| classForCoder | uint64 | self | 3003 |  |
| debugDescription | int32 | self | 3000 |  |
| finalize | int64 | self | 3001 |  |
| hash | uint32 | self | 3002 |  |

 

 



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

