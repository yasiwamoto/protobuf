# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [objectivec/Tests/unittest.proto](#objectivec_Tests_unittest-proto)
    - [BarRequest](#objc-protobuf-tests-BarRequest)
    - [BarResponse](#objc-protobuf-tests-BarResponse)
    - [BoolMessage](#objc-protobuf-tests-BoolMessage)
    - [BoolParseTester](#objc-protobuf-tests-BoolParseTester)
    - [EnumParseTester](#objc-protobuf-tests-EnumParseTester)
    - [FooClientMessage](#objc-protobuf-tests-FooClientMessage)
    - [FooRequest](#objc-protobuf-tests-FooRequest)
    - [FooResponse](#objc-protobuf-tests-FooResponse)
    - [FooServerMessage](#objc-protobuf-tests-FooServerMessage)
    - [ForeignMessage](#objc-protobuf-tests-ForeignMessage)
    - [Int32Message](#objc-protobuf-tests-Int32Message)
    - [Int64Message](#objc-protobuf-tests-Int64Message)
    - [ManyOptionalString](#objc-protobuf-tests-ManyOptionalString)
    - [MoreBytes](#objc-protobuf-tests-MoreBytes)
    - [MoreString](#objc-protobuf-tests-MoreString)
    - [NestedTestAllTypes](#objc-protobuf-tests-NestedTestAllTypes)
    - [OneBytes](#objc-protobuf-tests-OneBytes)
    - [OneString](#objc-protobuf-tests-OneString)
    - [OptionalGroup_extension](#objc-protobuf-tests-OptionalGroup_extension)
    - [RepeatedGroup_extension](#objc-protobuf-tests-RepeatedGroup_extension)
    - [SparseEnumMessage](#objc-protobuf-tests-SparseEnumMessage)
    - [TestAllExtensions](#objc-protobuf-tests-TestAllExtensions)
    - [TestAllTypes](#objc-protobuf-tests-TestAllTypes)
    - [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage)
    - [TestAllTypes.OptionalGroup](#objc-protobuf-tests-TestAllTypes-OptionalGroup)
    - [TestAllTypes.RepeatedGroup](#objc-protobuf-tests-TestAllTypes-RepeatedGroup)
    - [TestCamelCaseFieldNames](#objc-protobuf-tests-TestCamelCaseFieldNames)
    - [TestChildExtension](#objc-protobuf-tests-TestChildExtension)
    - [TestChildExtensionData](#objc-protobuf-tests-TestChildExtensionData)
    - [TestChildExtensionData.NestedTestAllExtensionsData](#objc-protobuf-tests-TestChildExtensionData-NestedTestAllExtensionsData)
    - [TestChildExtensionData.NestedTestAllExtensionsData.NestedDynamicExtensions](#objc-protobuf-tests-TestChildExtensionData-NestedTestAllExtensionsData-NestedDynamicExtensions)
    - [TestCommentInjectionMessage](#objc-protobuf-tests-TestCommentInjectionMessage)
    - [TestDeprecatedFields](#objc-protobuf-tests-TestDeprecatedFields)
    - [TestDeprecatedMessage](#objc-protobuf-tests-TestDeprecatedMessage)
    - [TestDupFieldNumber](#objc-protobuf-tests-TestDupFieldNumber)
    - [TestDupFieldNumber.Bar](#objc-protobuf-tests-TestDupFieldNumber-Bar)
    - [TestDupFieldNumber.Foo](#objc-protobuf-tests-TestDupFieldNumber-Foo)
    - [TestDynamicExtensions](#objc-protobuf-tests-TestDynamicExtensions)
    - [TestDynamicExtensions.DynamicMessageType](#objc-protobuf-tests-TestDynamicExtensions-DynamicMessageType)
    - [TestEagerMaybeLazy](#objc-protobuf-tests-TestEagerMaybeLazy)
    - [TestEagerMaybeLazy.NestedMessage](#objc-protobuf-tests-TestEagerMaybeLazy-NestedMessage)
    - [TestEagerMessage](#objc-protobuf-tests-TestEagerMessage)
    - [TestEmptyMessage](#objc-protobuf-tests-TestEmptyMessage)
    - [TestEmptyMessageWithExtensions](#objc-protobuf-tests-TestEmptyMessageWithExtensions)
    - [TestExtensionInsideTable](#objc-protobuf-tests-TestExtensionInsideTable)
    - [TestExtensionOrderings1](#objc-protobuf-tests-TestExtensionOrderings1)
    - [TestExtensionOrderings2](#objc-protobuf-tests-TestExtensionOrderings2)
    - [TestExtensionOrderings2.TestExtensionOrderings3](#objc-protobuf-tests-TestExtensionOrderings2-TestExtensionOrderings3)
    - [TestExtensionRangeSerialize](#objc-protobuf-tests-TestExtensionRangeSerialize)
    - [TestExtremeDefaultValues](#objc-protobuf-tests-TestExtremeDefaultValues)
    - [TestFieldOrderings](#objc-protobuf-tests-TestFieldOrderings)
    - [TestFieldOrderings.NestedMessage](#objc-protobuf-tests-TestFieldOrderings-NestedMessage)
    - [TestForeignNested](#objc-protobuf-tests-TestForeignNested)
    - [TestGroup](#objc-protobuf-tests-TestGroup)
    - [TestGroup.OptionalGroup](#objc-protobuf-tests-TestGroup-OptionalGroup)
    - [TestGroupExtension](#objc-protobuf-tests-TestGroupExtension)
    - [TestHugeFieldNumbers](#objc-protobuf-tests-TestHugeFieldNumbers)
    - [TestHugeFieldNumbers.OptionalGroup](#objc-protobuf-tests-TestHugeFieldNumbers-OptionalGroup)
    - [TestHugeFieldNumbers.StringStringMapEntry](#objc-protobuf-tests-TestHugeFieldNumbers-StringStringMapEntry)
    - [TestIsInitialized](#objc-protobuf-tests-TestIsInitialized)
    - [TestIsInitialized.SubMessage](#objc-protobuf-tests-TestIsInitialized-SubMessage)
    - [TestIsInitialized.SubMessage.SubGroup](#objc-protobuf-tests-TestIsInitialized-SubMessage-SubGroup)
    - [TestJsonName](#objc-protobuf-tests-TestJsonName)
    - [TestLazyMessage](#objc-protobuf-tests-TestLazyMessage)
    - [TestMergeException](#objc-protobuf-tests-TestMergeException)
    - [TestMessageSize](#objc-protobuf-tests-TestMessageSize)
    - [TestMixedFieldsAndExtensions](#objc-protobuf-tests-TestMixedFieldsAndExtensions)
    - [TestMultipleExtensionRanges](#objc-protobuf-tests-TestMultipleExtensionRanges)
    - [TestMutualRecursionA](#objc-protobuf-tests-TestMutualRecursionA)
    - [TestMutualRecursionA.SubGroup](#objc-protobuf-tests-TestMutualRecursionA-SubGroup)
    - [TestMutualRecursionA.SubMessage](#objc-protobuf-tests-TestMutualRecursionA-SubMessage)
    - [TestMutualRecursionB](#objc-protobuf-tests-TestMutualRecursionB)
    - [TestNestedChildExtension](#objc-protobuf-tests-TestNestedChildExtension)
    - [TestNestedChildExtensionData](#objc-protobuf-tests-TestNestedChildExtensionData)
    - [TestNestedExtension](#objc-protobuf-tests-TestNestedExtension)
    - [TestNestedExtension.OptionalGroup_extension](#objc-protobuf-tests-TestNestedExtension-OptionalGroup_extension)
    - [TestNestedGroupExtensionInnerExtension](#objc-protobuf-tests-TestNestedGroupExtensionInnerExtension)
    - [TestNestedGroupExtensionOuter](#objc-protobuf-tests-TestNestedGroupExtensionOuter)
    - [TestNestedGroupExtensionOuter.Layer1OptionalGroup](#objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup)
    - [TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2AnotherOptionalRepeatedGroup](#objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup-Layer2AnotherOptionalRepeatedGroup)
    - [TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2RepeatedGroup](#objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup-Layer2RepeatedGroup)
    - [TestNestedMessageHasBits](#objc-protobuf-tests-TestNestedMessageHasBits)
    - [TestNestedMessageHasBits.NestedMessage](#objc-protobuf-tests-TestNestedMessageHasBits-NestedMessage)
    - [TestNestedRequiredForeign](#objc-protobuf-tests-TestNestedRequiredForeign)
    - [TestOneof](#objc-protobuf-tests-TestOneof)
    - [TestOneof.FooGroup](#objc-protobuf-tests-TestOneof-FooGroup)
    - [TestOneof2](#objc-protobuf-tests-TestOneof2)
    - [TestOneof2.FooGroup](#objc-protobuf-tests-TestOneof2-FooGroup)
    - [TestOneof2.NestedMessage](#objc-protobuf-tests-TestOneof2-NestedMessage)
    - [TestOneofBackwardsCompatible](#objc-protobuf-tests-TestOneofBackwardsCompatible)
    - [TestOneofBackwardsCompatible.FooGroup](#objc-protobuf-tests-TestOneofBackwardsCompatible-FooGroup)
    - [TestPackedExtensions](#objc-protobuf-tests-TestPackedExtensions)
    - [TestPackedTypes](#objc-protobuf-tests-TestPackedTypes)
    - [TestParsingMerge](#objc-protobuf-tests-TestParsingMerge)
    - [TestParsingMerge.OptionalGroup](#objc-protobuf-tests-TestParsingMerge-OptionalGroup)
    - [TestParsingMerge.RepeatedFieldsGenerator](#objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator)
    - [TestParsingMerge.RepeatedFieldsGenerator.Group1](#objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator-Group1)
    - [TestParsingMerge.RepeatedFieldsGenerator.Group2](#objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator-Group2)
    - [TestParsingMerge.RepeatedGroup](#objc-protobuf-tests-TestParsingMerge-RepeatedGroup)
    - [TestPickleNestedMessage](#objc-protobuf-tests-TestPickleNestedMessage)
    - [TestPickleNestedMessage.NestedMessage](#objc-protobuf-tests-TestPickleNestedMessage-NestedMessage)
    - [TestPickleNestedMessage.NestedMessage.NestedNestedMessage](#objc-protobuf-tests-TestPickleNestedMessage-NestedMessage-NestedNestedMessage)
    - [TestReallyLargeTagNumber](#objc-protobuf-tests-TestReallyLargeTagNumber)
    - [TestRecursiveMessage](#objc-protobuf-tests-TestRecursiveMessage)
    - [TestRepeatedScalarDifferentTagSizes](#objc-protobuf-tests-TestRepeatedScalarDifferentTagSizes)
    - [TestRequired](#objc-protobuf-tests-TestRequired)
    - [TestRequiredForeign](#objc-protobuf-tests-TestRequiredForeign)
    - [TestRequiredMessage](#objc-protobuf-tests-TestRequiredMessage)
    - [TestRequiredOneof](#objc-protobuf-tests-TestRequiredOneof)
    - [TestRequiredOneof.NestedMessage](#objc-protobuf-tests-TestRequiredOneof-NestedMessage)
    - [TestReservedFields](#objc-protobuf-tests-TestReservedFields)
    - [TestUnpackedExtensions](#objc-protobuf-tests-TestUnpackedExtensions)
    - [TestUnpackedTypes](#objc-protobuf-tests-TestUnpackedTypes)
    - [TestVerifyBigFieldNumberUint32](#objc-protobuf-tests-TestVerifyBigFieldNumberUint32)
    - [TestVerifyBigFieldNumberUint32.Nested](#objc-protobuf-tests-TestVerifyBigFieldNumberUint32-Nested)
    - [TestVerifyInt32](#objc-protobuf-tests-TestVerifyInt32)
    - [TestVerifyInt32BigFieldNumber](#objc-protobuf-tests-TestVerifyInt32BigFieldNumber)
    - [TestVerifyInt32Simple](#objc-protobuf-tests-TestVerifyInt32Simple)
    - [TestVerifyMostlyInt32](#objc-protobuf-tests-TestVerifyMostlyInt32)
    - [TestVerifyMostlyInt32BigFieldNumber](#objc-protobuf-tests-TestVerifyMostlyInt32BigFieldNumber)
    - [TestVerifyOneInt32BigFieldNumber](#objc-protobuf-tests-TestVerifyOneInt32BigFieldNumber)
    - [TestVerifyOneUint32](#objc-protobuf-tests-TestVerifyOneUint32)
    - [TestVerifyUint32](#objc-protobuf-tests-TestVerifyUint32)
    - [TestVerifyUint32BigFieldNumber](#objc-protobuf-tests-TestVerifyUint32BigFieldNumber)
    - [TestVerifyUint32Simple](#objc-protobuf-tests-TestVerifyUint32Simple)
    - [Uint32Message](#objc-protobuf-tests-Uint32Message)
    - [Uint64Message](#objc-protobuf-tests-Uint64Message)
  
    - [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary)
    - [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge)
    - [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0)
    - [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1)
    - [ForeignEnum](#objc-protobuf-tests-ForeignEnum)
    - [TestAllTypes.NestedEnum](#objc-protobuf-tests-TestAllTypes-NestedEnum)
    - [TestDynamicExtensions.DynamicEnumType](#objc-protobuf-tests-TestDynamicExtensions-DynamicEnumType)
    - [TestEnumWithDupValue](#objc-protobuf-tests-TestEnumWithDupValue)
    - [TestOneof2.NestedEnum](#objc-protobuf-tests-TestOneof2-NestedEnum)
    - [TestReservedEnumFields](#objc-protobuf-tests-TestReservedEnumFields)
    - [TestSparseEnum](#objc-protobuf-tests-TestSparseEnum)
    - [VeryLargeEnum](#objc-protobuf-tests-VeryLargeEnum)
  
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
    - [File-level Extensions](#objectivec_Tests_unittest-proto-extensions)
  
    - [TestService](#objc-protobuf-tests-TestService)
  
- [Scalar Value Types](#scalar-value-types)



<a name="objectivec_Tests_unittest-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objectivec/Tests/unittest.proto



<a name="objc-protobuf-tests-BarRequest"></a>

### BarRequest







<a name="objc-protobuf-tests-BarResponse"></a>

### BarResponse







<a name="objc-protobuf-tests-BoolMessage"></a>

### BoolMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [bool](#bool) | optional |  |






<a name="objc-protobuf-tests-BoolParseTester"></a>

### BoolParseTester
This message contains different kind of bool fields to exercise the different
parsers in table-drived.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_bool_lowfield | [bool](#bool) | optional |  |
| optional_bool_midfield | [bool](#bool) | optional |  |
| optional_bool_hifield | [bool](#bool) | optional |  |
| repeated_bool_lowfield | [bool](#bool) | repeated |  |
| repeated_bool_midfield | [bool](#bool) | repeated |  |
| repeated_bool_hifield | [bool](#bool) | repeated |  |
| packed_bool_lowfield | [bool](#bool) | repeated |  |
| packed_bool_midfield | [bool](#bool) | repeated |  |
| packed_bool_hifield | [bool](#bool) | repeated |  |
| other_field | [int32](#int32) | optional | An arbitrary field we can append to to break the runs of repeated fields. |






<a name="objc-protobuf-tests-EnumParseTester"></a>

### EnumParseTester
This message contains different kind of enums to exercise the different
parsers in table-driven.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_seq_small_0_lowfield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | optional |  |
| optional_seq_small_0_midfield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | optional |  |
| optional_seq_small_0_hifield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | optional |  |
| repeated_seq_small_0_lowfield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | repeated |  |
| repeated_seq_small_0_midfield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | repeated |  |
| repeated_seq_small_0_hifield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | repeated |  |
| packed_seq_small_0_lowfield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | repeated |  |
| packed_seq_small_0_midfield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | repeated |  |
| packed_seq_small_0_hifield | [EnumParseTester.SeqSmall0](#objc-protobuf-tests-EnumParseTester-SeqSmall0) | repeated |  |
| optional_seq_small_1_lowfield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | optional |  |
| optional_seq_small_1_midfield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | optional |  |
| optional_seq_small_1_hifield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | optional |  |
| repeated_seq_small_1_lowfield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | repeated |  |
| repeated_seq_small_1_midfield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | repeated |  |
| repeated_seq_small_1_hifield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | repeated |  |
| packed_seq_small_1_lowfield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | repeated |  |
| packed_seq_small_1_midfield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | repeated |  |
| packed_seq_small_1_hifield | [EnumParseTester.SeqSmall1](#objc-protobuf-tests-EnumParseTester-SeqSmall1) | repeated |  |
| optional_seq_large_lowfield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | optional |  |
| optional_seq_large_midfield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | optional |  |
| optional_seq_large_hifield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | optional |  |
| repeated_seq_large_lowfield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | repeated |  |
| repeated_seq_large_midfield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | repeated |  |
| repeated_seq_large_hifield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | repeated |  |
| packed_seq_large_lowfield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | repeated |  |
| packed_seq_large_midfield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | repeated |  |
| packed_seq_large_hifield | [EnumParseTester.SeqLarge](#objc-protobuf-tests-EnumParseTester-SeqLarge) | repeated |  |
| optional_arbitrary_lowfield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | optional |  |
| optional_arbitrary_midfield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | optional |  |
| optional_arbitrary_hifield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | optional |  |
| repeated_arbitrary_lowfield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | repeated |  |
| repeated_arbitrary_midfield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | repeated |  |
| repeated_arbitrary_hifield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | repeated |  |
| packed_arbitrary_lowfield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | repeated |  |
| packed_arbitrary_midfield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | repeated |  |
| packed_arbitrary_hifield | [EnumParseTester.Arbitrary](#objc-protobuf-tests-EnumParseTester-Arbitrary) | repeated |  |
| other_field | [int32](#int32) | optional | An arbitrary field we can append to to break the runs of repeated fields. |






<a name="objc-protobuf-tests-FooClientMessage"></a>

### FooClientMessage







<a name="objc-protobuf-tests-FooRequest"></a>

### FooRequest
Test that RPC services work.






<a name="objc-protobuf-tests-FooResponse"></a>

### FooResponse







<a name="objc-protobuf-tests-FooServerMessage"></a>

### FooServerMessage







<a name="objc-protobuf-tests-ForeignMessage"></a>

### ForeignMessage
Define these after TestAllTypes to make sure the compiler can handle
that.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| c | [int32](#int32) | optional |  |
| d | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-Int32Message"></a>

### Int32Message
Test int32, uint32, int64, uint64, and bool are all compatible


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-Int64Message"></a>

### Int64Message



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [int64](#int64) | optional |  |






<a name="objc-protobuf-tests-ManyOptionalString"></a>

### ManyOptionalString



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| str1 | [string](#string) | optional |  |
| str2 | [string](#string) | optional |  |
| str3 | [string](#string) | optional |  |
| str4 | [string](#string) | optional |  |
| str5 | [string](#string) | optional |  |
| str6 | [string](#string) | optional |  |
| str7 | [string](#string) | optional |  |
| str8 | [string](#string) | optional |  |
| str9 | [string](#string) | optional |  |
| str10 | [string](#string) | optional |  |
| str11 | [string](#string) | optional |  |
| str12 | [string](#string) | optional |  |
| str13 | [string](#string) | optional |  |
| str14 | [string](#string) | optional |  |
| str15 | [string](#string) | optional |  |
| str16 | [string](#string) | optional |  |
| str17 | [string](#string) | optional |  |
| str18 | [string](#string) | optional |  |
| str19 | [string](#string) | optional |  |
| str20 | [string](#string) | optional |  |
| str21 | [string](#string) | optional |  |
| str22 | [string](#string) | optional |  |
| str23 | [string](#string) | optional |  |
| str24 | [string](#string) | optional |  |
| str25 | [string](#string) | optional |  |
| str26 | [string](#string) | optional |  |
| str27 | [string](#string) | optional |  |
| str28 | [string](#string) | optional |  |
| str29 | [string](#string) | optional |  |
| str30 | [string](#string) | optional |  |
| str31 | [string](#string) | optional |  |
| str32 | [string](#string) | optional |  |






<a name="objc-protobuf-tests-MoreBytes"></a>

### MoreBytes



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [bytes](#bytes) | repeated |  |






<a name="objc-protobuf-tests-MoreString"></a>

### MoreString



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [string](#string) | repeated |  |






<a name="objc-protobuf-tests-NestedTestAllTypes"></a>

### NestedTestAllTypes
This proto includes a recursively nested message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| child | [NestedTestAllTypes](#objc-protobuf-tests-NestedTestAllTypes) | optional |  |
| payload | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_child | [NestedTestAllTypes](#objc-protobuf-tests-NestedTestAllTypes) | repeated |  |
| lazy_child | [NestedTestAllTypes](#objc-protobuf-tests-NestedTestAllTypes) | optional |  |
| eager_child | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-OneBytes"></a>

### OneBytes



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [bytes](#bytes) | optional |  |






<a name="objc-protobuf-tests-OneString"></a>

### OneString
Test String and Bytes: string is for valid UTF-8 strings


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [string](#string) | optional |  |






<a name="objc-protobuf-tests-OptionalGroup_extension"></a>

### OptionalGroup_extension



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-RepeatedGroup_extension"></a>

### RepeatedGroup_extension



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-SparseEnumMessage"></a>

### SparseEnumMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| sparse_enum | [TestSparseEnum](#objc-protobuf-tests-TestSparseEnum) | optional |  |






<a name="objc-protobuf-tests-TestAllExtensions"></a>

### TestAllExtensions







<a name="objc-protobuf-tests-TestAllTypes"></a>

### TestAllTypes
This proto includes every type of field in both singular and repeated
forms.


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
| optionalgroup | [TestAllTypes.OptionalGroup](#objc-protobuf-tests-TestAllTypes-OptionalGroup) | optional |  |
| optional_nested_message | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | optional |  |
| optional_foreign_message | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | optional |  |
| optional_import_message | [import.Message](#objc-protobuf-tests-import-Message) | optional |  |
| optional_nested_enum | [TestAllTypes.NestedEnum](#objc-protobuf-tests-TestAllTypes-NestedEnum) | optional |  |
| optional_foreign_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | optional |  |
| optional_import_enum | [import.Enum](#objc-protobuf-tests-import-Enum) | optional |  |
| optional_string_piece | [string](#string) | optional |  |
| optional_cord | [string](#string) | optional |  |
| optional_public_import_message | [public_import.Message](#objc-protobuf-tests-public_import-Message) | optional | Defined in unittest_import_public.proto |
| optional_lazy_message | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | optional |  |
| optional_unverified_lazy_message | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | optional |  |
| repeated_int32 | [int32](#int32) | repeated | Repeated |
| repeated_int64 | [int64](#int64) | repeated |  |
| repeated_uint32 | [uint32](#uint32) | repeated |  |
| repeated_uint64 | [uint64](#uint64) | repeated |  |
| repeated_sint32 | [sint32](#sint32) | repeated |  |
| repeated_sint64 | [sint64](#sint64) | repeated |  |
| repeated_fixed32 | [fixed32](#fixed32) | repeated |  |
| repeated_fixed64 | [fixed64](#fixed64) | repeated |  |
| repeated_sfixed32 | [sfixed32](#sfixed32) | repeated |  |
| repeated_sfixed64 | [sfixed64](#sfixed64) | repeated |  |
| repeated_float | [float](#float) | repeated |  |
| repeated_double | [double](#double) | repeated |  |
| repeated_bool | [bool](#bool) | repeated |  |
| repeated_string | [string](#string) | repeated |  |
| repeated_bytes | [bytes](#bytes) | repeated |  |
| repeatedgroup | [TestAllTypes.RepeatedGroup](#objc-protobuf-tests-TestAllTypes-RepeatedGroup) | repeated |  |
| repeated_nested_message | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | repeated |  |
| repeated_foreign_message | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | repeated |  |
| repeated_import_message | [import.Message](#objc-protobuf-tests-import-Message) | repeated |  |
| repeated_nested_enum | [TestAllTypes.NestedEnum](#objc-protobuf-tests-TestAllTypes-NestedEnum) | repeated |  |
| repeated_foreign_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | repeated |  |
| repeated_import_enum | [import.Enum](#objc-protobuf-tests-import-Enum) | repeated |  |
| repeated_string_piece | [string](#string) | repeated |  |
| repeated_cord | [string](#string) | repeated |  |
| repeated_lazy_message | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | repeated |  |
| default_int32 | [int32](#int32) | optional | Singular with defaults Default: 41 |
| default_int64 | [int64](#int64) | optional |  Default: 42 |
| default_uint32 | [uint32](#uint32) | optional |  Default: 43 |
| default_uint64 | [uint64](#uint64) | optional |  Default: 44 |
| default_sint32 | [sint32](#sint32) | optional |  Default: -45 |
| default_sint64 | [sint64](#sint64) | optional |  Default: 46 |
| default_fixed32 | [fixed32](#fixed32) | optional |  Default: 47 |
| default_fixed64 | [fixed64](#fixed64) | optional |  Default: 48 |
| default_sfixed32 | [sfixed32](#sfixed32) | optional |  Default: 49 |
| default_sfixed64 | [sfixed64](#sfixed64) | optional |  Default: -50 |
| default_float | [float](#float) | optional |  Default: 51.5 |
| default_double | [double](#double) | optional |  Default: 52000 |
| default_bool | [bool](#bool) | optional |  Default: true |
| default_string | [string](#string) | optional |  Default: hello |
| default_bytes | [bytes](#bytes) | optional |  Default: world |
| default_nested_enum | [TestAllTypes.NestedEnum](#objc-protobuf-tests-TestAllTypes-NestedEnum) | optional |  Default: BAR |
| default_foreign_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | optional |  Default: FOREIGN_BAR |
| default_import_enum | [import.Enum](#objc-protobuf-tests-import-Enum) | optional |  Default: IMPORT_BAR |
| default_string_piece | [string](#string) | optional |  Default: abc |
| default_cord | [string](#string) | optional |  Default: 123 |
| oneof_uint32 | [uint32](#uint32) | optional |  |
| oneof_nested_message | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | optional |  |
| oneof_string | [string](#string) | optional |  |
| oneof_bytes | [bytes](#bytes) | optional |  |






<a name="objc-protobuf-tests-TestAllTypes-NestedMessage"></a>

### TestAllTypes.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bb | [int32](#int32) | optional | The field name &#34;b&#34; fails to compile in proto1 because it conflicts with a local variable named &#34;b&#34; in one of the generated methods. Doh. This file needs to compile in proto1 to test backwards-compatibility. |






<a name="objc-protobuf-tests-TestAllTypes-OptionalGroup"></a>

### TestAllTypes.OptionalGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestAllTypes-RepeatedGroup"></a>

### TestAllTypes.RepeatedGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestCamelCaseFieldNames"></a>

### TestCamelCaseFieldNames
Test message with CamelCase field names.  This violates Protocol Buffer
standard style.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| PrimitiveField | [int32](#int32) | optional |  |
| StringField | [string](#string) | optional |  |
| EnumField | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | optional |  |
| MessageField | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | optional |  |
| StringPieceField | [string](#string) | optional |  |
| CordField | [string](#string) | optional |  |
| RepeatedPrimitiveField | [int32](#int32) | repeated |  |
| RepeatedStringField | [string](#string) | repeated |  |
| RepeatedEnumField | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | repeated |  |
| RepeatedMessageField | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | repeated |  |
| RepeatedStringPieceField | [string](#string) | repeated |  |
| RepeatedCordField | [string](#string) | repeated |  |






<a name="objc-protobuf-tests-TestChildExtension"></a>

### TestChildExtension



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [string](#string) | optional |  |
| b | [string](#string) | optional |  |
| optional_extension | [TestAllExtensions](#objc-protobuf-tests-TestAllExtensions) | optional |  |






<a name="objc-protobuf-tests-TestChildExtensionData"></a>

### TestChildExtensionData
Emulates wireformat data of TestChildExtension with dynamic extension
(DynamicExtension).


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [string](#string) | optional |  |
| b | [string](#string) | optional |  |
| optional_extension | [TestChildExtensionData.NestedTestAllExtensionsData](#objc-protobuf-tests-TestChildExtensionData-NestedTestAllExtensionsData) | optional |  |






<a name="objc-protobuf-tests-TestChildExtensionData-NestedTestAllExtensionsData"></a>

### TestChildExtensionData.NestedTestAllExtensionsData



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| dynamic | [TestChildExtensionData.NestedTestAllExtensionsData.NestedDynamicExtensions](#objc-protobuf-tests-TestChildExtensionData-NestedTestAllExtensionsData-NestedDynamicExtensions) | optional |  |






<a name="objc-protobuf-tests-TestChildExtensionData-NestedTestAllExtensionsData-NestedDynamicExtensions"></a>

### TestChildExtensionData.NestedTestAllExtensionsData.NestedDynamicExtensions



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| b | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestCommentInjectionMessage"></a>

### TestCommentInjectionMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [string](#string) | optional | &lt;- This should not close the generated doc comment Default: */ &lt;- Neither should this. |






<a name="objc-protobuf-tests-TestDeprecatedFields"></a>

### TestDeprecatedFields



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| deprecated_int32 | [int32](#int32) | optional | **Deprecated.**  |
| deprecated_int32_in_oneof | [int32](#int32) | optional | **Deprecated.**  |






<a name="objc-protobuf-tests-TestDeprecatedMessage"></a>

### TestDeprecatedMessage







<a name="objc-protobuf-tests-TestDupFieldNumber"></a>

### TestDupFieldNumber
Test that groups have disjoint field numbers from their siblings and
parents.  This is NOT possible in proto1; only google.protobuf.  When attempting
to compile with proto1, this will emit an error; so we only include it
in objc.protobuf.tests_proto.

NO_PROTO1


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional | NO_PROTO1 |
| foo | [TestDupFieldNumber.Foo](#objc-protobuf-tests-TestDupFieldNumber-Foo) | optional |  |
| bar | [TestDupFieldNumber.Bar](#objc-protobuf-tests-TestDupFieldNumber-Bar) | optional |  |






<a name="objc-protobuf-tests-TestDupFieldNumber-Bar"></a>

### TestDupFieldNumber.Bar



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestDupFieldNumber-Foo"></a>

### TestDupFieldNumber.Foo



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestDynamicExtensions"></a>

### TestDynamicExtensions
Used by ExtensionSetTest/DynamicExtensions.  The test actually builds
a set of extensions to TestAllExtensions dynamically, based on the fields
of this message type.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| scalar_extension | [fixed32](#fixed32) | optional |  |
| enum_extension | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | optional |  |
| dynamic_enum_extension | [TestDynamicExtensions.DynamicEnumType](#objc-protobuf-tests-TestDynamicExtensions-DynamicEnumType) | optional |  |
| message_extension | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | optional |  |
| dynamic_message_extension | [TestDynamicExtensions.DynamicMessageType](#objc-protobuf-tests-TestDynamicExtensions-DynamicMessageType) | optional |  |
| repeated_extension | [string](#string) | repeated |  |
| packed_extension | [sint32](#sint32) | repeated |  |






<a name="objc-protobuf-tests-TestDynamicExtensions-DynamicMessageType"></a>

### TestDynamicExtensions.DynamicMessageType



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| dynamic_field | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestEagerMaybeLazy"></a>

### TestEagerMaybeLazy



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| message_foo | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| message_bar | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| message_baz | [TestEagerMaybeLazy.NestedMessage](#objc-protobuf-tests-TestEagerMaybeLazy-NestedMessage) | optional |  |






<a name="objc-protobuf-tests-TestEagerMaybeLazy-NestedMessage"></a>

### TestEagerMaybeLazy.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| packed | [TestPackedTypes](#objc-protobuf-tests-TestPackedTypes) | optional |  |






<a name="objc-protobuf-tests-TestEagerMessage"></a>

### TestEagerMessage
Additional messages for testing lazy fields.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| sub_message | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestEmptyMessage"></a>

### TestEmptyMessage
TestEmptyMessage is used to test unknown field support.






<a name="objc-protobuf-tests-TestEmptyMessageWithExtensions"></a>

### TestEmptyMessageWithExtensions
Like above, but declare all field numbers as potential extensions.  No
actual extensions should ever be defined for this type.






<a name="objc-protobuf-tests-TestExtensionInsideTable"></a>

### TestExtensionInsideTable



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field1 | [int32](#int32) | optional |  |
| field2 | [int32](#int32) | optional |  |
| field3 | [int32](#int32) | optional |  |
| field4 | [int32](#int32) | optional |  |
| field6 | [int32](#int32) | optional |  |
| field7 | [int32](#int32) | optional |  |
| field8 | [int32](#int32) | optional |  |
| field9 | [int32](#int32) | optional |  |
| field10 | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestExtensionOrderings1"></a>

### TestExtensionOrderings1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| my_string | [string](#string) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| test_ext_orderings1 | TestExtensionOrderings1 | TestFieldOrderings | 13 |  |




<a name="objc-protobuf-tests-TestExtensionOrderings2"></a>

### TestExtensionOrderings2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| my_string | [string](#string) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| test_ext_orderings2 | TestExtensionOrderings2 | TestFieldOrderings | 12 |  |




<a name="objc-protobuf-tests-TestExtensionOrderings2-TestExtensionOrderings3"></a>

### TestExtensionOrderings2.TestExtensionOrderings3



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| my_string | [string](#string) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| test_ext_orderings3 | TestExtensionOrderings2.TestExtensionOrderings3 | TestFieldOrderings | 14 |  |




<a name="objc-protobuf-tests-TestExtensionRangeSerialize"></a>

### TestExtensionRangeSerialize



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo_one | [int32](#int32) | optional |  |
| foo_two | [int32](#int32) | optional |  |
| foo_three | [int32](#int32) | optional |  |
| foo_four | [int32](#int32) | optional |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| bar_one | int32 | TestExtensionRangeSerialize | 2 |  |
| bar_two | int32 | TestExtensionRangeSerialize | 4 |  |
| bar_three | int32 | TestExtensionRangeSerialize | 10 |  |
| bar_four | int32 | TestExtensionRangeSerialize | 15 |  |
| bar_five | int32 | TestExtensionRangeSerialize | 19 |  |




<a name="objc-protobuf-tests-TestExtremeDefaultValues"></a>

### TestExtremeDefaultValues



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| escaped_bytes | [bytes](#bytes) | optional |  Default: \000\001\007\010\014\n\r\t\013\\\&#39;\&#34;\376 |
| large_uint32 | [uint32](#uint32) | optional |  Default: 4294967295 |
| large_uint64 | [uint64](#uint64) | optional |  Default: 18446744073709551615 |
| small_int32 | [int32](#int32) | optional |  Default: -2147483647 |
| small_int64 | [int64](#int64) | optional |  Default: -9223372036854775807 |
| really_small_int32 | [int32](#int32) | optional |  Default: -2147483648 |
| really_small_int64 | [int64](#int64) | optional |  Default: -9223372036854775808 |
| utf8_string | [string](#string) | optional | The default value here is UTF-8 for &#34;\u1234&#34;. (We could also just type the UTF-8 text directly into this text file rather than escape it, but lots of people use editors that would be confused by this.) Default: ሴ |
| zero_float | [float](#float) | optional | Tests for single-precision floating-point values. Default: 0 |
| one_float | [float](#float) | optional |  Default: 1 |
| small_float | [float](#float) | optional |  Default: 1.5 |
| negative_one_float | [float](#float) | optional |  Default: -1 |
| negative_float | [float](#float) | optional |  Default: -1.5 |
| large_float | [float](#float) | optional | Using exponents Default: 2e&#43;08 |
| small_negative_float | [float](#float) | optional |  Default: -8e-28 |
| inf_double | [double](#double) | optional | Text for nonfinite floating-point values. Default: inf |
| neg_inf_double | [double](#double) | optional |  Default: -inf |
| nan_double | [double](#double) | optional |  Default: nan |
| inf_float | [float](#float) | optional |  Default: inf |
| neg_inf_float | [float](#float) | optional |  Default: -inf |
| nan_float | [float](#float) | optional |  Default: nan |
| cpp_trigraph | [string](#string) | optional | Tests for C&#43;&#43; trigraphs. Trigraphs should be escaped in C&#43;&#43; generated files, but they should not be escaped for other languages. Note that in .proto file, &#34;\?&#34; is a valid way to escape ? in string literals. Default: ? ? ?? ?? ??? ??/ ??- |
| string_with_zero | [string](#string) | optional | String defaults containing the character &#39;\000&#39; Default: hel�lo |
| bytes_with_zero | [bytes](#bytes) | optional |  Default: wor\000ld |
| string_piece_with_zero | [string](#string) | optional |  Default: ab�c |
| cord_with_zero | [string](#string) | optional |  Default: 12�3 |
| replacement_string | [string](#string) | optional |  Default: ${unknown} |






<a name="objc-protobuf-tests-TestFieldOrderings"></a>

### TestFieldOrderings
We list fields out of order, to ensure that we&#39;re using field number and not
field index to determine serialization order.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| my_string | [string](#string) | optional |  |
| my_int | [int64](#int64) | optional |  |
| my_float | [float](#float) | optional |  |
| optional_nested_message | [TestFieldOrderings.NestedMessage](#objc-protobuf-tests-TestFieldOrderings-NestedMessage) | optional |  |






<a name="objc-protobuf-tests-TestFieldOrderings-NestedMessage"></a>

### TestFieldOrderings.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| oo | [int64](#int64) | optional |  |
| bb | [int32](#int32) | optional | The field name &#34;b&#34; fails to compile in proto1 because it conflicts with a local variable named &#34;b&#34; in one of the generated methods. Doh. This file needs to compile in proto1 to test backwards-compatibility. |






<a name="objc-protobuf-tests-TestForeignNested"></a>

### TestForeignNested
Test that we can use NestedMessage from outside TestAllTypes.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foreign_nested | [TestAllTypes.NestedMessage](#objc-protobuf-tests-TestAllTypes-NestedMessage) | optional |  |






<a name="objc-protobuf-tests-TestGroup"></a>

### TestGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optionalgroup | [TestGroup.OptionalGroup](#objc-protobuf-tests-TestGroup-OptionalGroup) | optional |  |
| optional_foreign_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | optional |  |






<a name="objc-protobuf-tests-TestGroup-OptionalGroup"></a>

### TestGroup.OptionalGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestGroupExtension"></a>

### TestGroupExtension







<a name="objc-protobuf-tests-TestHugeFieldNumbers"></a>

### TestHugeFieldNumbers



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32 | [int32](#int32) | optional |  |
| fixed_32 | [int32](#int32) | optional |  |
| repeated_int32 | [int32](#int32) | repeated |  |
| packed_int32 | [int32](#int32) | repeated |  |
| optional_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | optional |  |
| optional_string | [string](#string) | optional |  |
| optional_bytes | [bytes](#bytes) | optional |  |
| optional_message | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | optional |  |
| optionalgroup | [TestHugeFieldNumbers.OptionalGroup](#objc-protobuf-tests-TestHugeFieldNumbers-OptionalGroup) | optional |  |
| string_string_map | [TestHugeFieldNumbers.StringStringMapEntry](#objc-protobuf-tests-TestHugeFieldNumbers-StringStringMapEntry) | repeated |  |
| oneof_uint32 | [uint32](#uint32) | optional |  |
| oneof_test_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| oneof_string | [string](#string) | optional |  |
| oneof_bytes | [bytes](#bytes) | optional |  |






<a name="objc-protobuf-tests-TestHugeFieldNumbers-OptionalGroup"></a>

### TestHugeFieldNumbers.OptionalGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestHugeFieldNumbers-StringStringMapEntry"></a>

### TestHugeFieldNumbers.StringStringMapEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestIsInitialized"></a>

### TestIsInitialized



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| sub_message | [TestIsInitialized.SubMessage](#objc-protobuf-tests-TestIsInitialized-SubMessage) | optional |  |






<a name="objc-protobuf-tests-TestIsInitialized-SubMessage"></a>

### TestIsInitialized.SubMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| subgroup | [TestIsInitialized.SubMessage.SubGroup](#objc-protobuf-tests-TestIsInitialized-SubMessage-SubGroup) | optional |  |






<a name="objc-protobuf-tests-TestIsInitialized-SubMessage-SubGroup"></a>

### TestIsInitialized.SubMessage.SubGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| i | [int32](#int32) | required |  |






<a name="objc-protobuf-tests-TestJsonName"></a>

### TestJsonName



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_name1 | [int32](#int32) | optional |  |
| fieldName2 | [int32](#int32) | optional |  |
| FieldName3 | [int32](#int32) | optional |  |
| _field_name4 | [int32](#int32) | optional |  |
| FIELD_NAME5 | [int32](#int32) | optional |  |
| field_name6 | [int32](#int32) | optional |  |
| fieldname7 | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestLazyMessage"></a>

### TestLazyMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| sub_message | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestMergeException"></a>

### TestMergeException
Test that the correct exception is thrown by parseFrom in a corner case
involving merging, extensions, and required fields.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| all_extensions | [TestAllExtensions](#objc-protobuf-tests-TestAllExtensions) | optional |  |






<a name="objc-protobuf-tests-TestMessageSize"></a>

### TestMessageSize
Used to check that the c&#43;&#43; code generator re-orders messages to reduce
padding.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| m1 | [bool](#bool) | optional |  |
| m2 | [int64](#int64) | optional |  |
| m3 | [bool](#bool) | optional |  |
| m4 | [string](#string) | optional |  |
| m5 | [int32](#int32) | optional |  |
| m6 | [int64](#int64) | optional |  |






<a name="objc-protobuf-tests-TestMixedFieldsAndExtensions"></a>

### TestMixedFieldsAndExtensions



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| b | [fixed32](#fixed32) | repeated |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| c | int32 | TestMixedFieldsAndExtensions | 2 |  |
| d | fixed32 | TestMixedFieldsAndExtensions | 4 |  |




<a name="objc-protobuf-tests-TestMultipleExtensionRanges"></a>

### TestMultipleExtensionRanges







<a name="objc-protobuf-tests-TestMutualRecursionA"></a>

### TestMutualRecursionA
Test that mutual recursion works.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bb | [TestMutualRecursionB](#objc-protobuf-tests-TestMutualRecursionB) | optional |  |
| subgroup | [TestMutualRecursionA.SubGroup](#objc-protobuf-tests-TestMutualRecursionA-SubGroup) | optional |  |






<a name="objc-protobuf-tests-TestMutualRecursionA-SubGroup"></a>

### TestMutualRecursionA.SubGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| sub_message | [TestMutualRecursionA.SubMessage](#objc-protobuf-tests-TestMutualRecursionA-SubMessage) | optional | Needed because of bug in javatest |
| not_in_this_scc | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestMutualRecursionA-SubMessage"></a>

### TestMutualRecursionA.SubMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| b | [TestMutualRecursionB](#objc-protobuf-tests-TestMutualRecursionB) | optional |  |






<a name="objc-protobuf-tests-TestMutualRecursionB"></a>

### TestMutualRecursionB



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [TestMutualRecursionA](#objc-protobuf-tests-TestMutualRecursionA) | optional |  |
| optional_int32 | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestNestedChildExtension"></a>

### TestNestedChildExtension



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| child | [TestChildExtension](#objc-protobuf-tests-TestChildExtension) | optional |  |






<a name="objc-protobuf-tests-TestNestedChildExtensionData"></a>

### TestNestedChildExtensionData
Emulates wireformat data of TestNestedChildExtension with dynamic extension
(DynamicExtension).


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| child | [TestChildExtensionData](#objc-protobuf-tests-TestChildExtensionData) | optional |  |






<a name="objc-protobuf-tests-TestNestedExtension"></a>

### TestNestedExtension





| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| test | string | TestAllExtensions | 1002 | Check for bug where string extensions declared in tested scope did not compile. Default: test |
| nested_string_extension | string | TestAllExtensions | 1003 | Used to test if generated extension name is correct when there are underscores. |
| optionalgroup_extension | TestNestedExtension.OptionalGroup_extension | TestGroupExtension | 16 |  |
| optional_foreign_enum_extension | ForeignEnum | TestGroupExtension | 22 |  |




<a name="objc-protobuf-tests-TestNestedExtension-OptionalGroup_extension"></a>

### TestNestedExtension.OptionalGroup_extension



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestNestedGroupExtensionInnerExtension"></a>

### TestNestedGroupExtensionInnerExtension



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| inner_name | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestNestedGroupExtensionOuter"></a>

### TestNestedGroupExtensionOuter
NOTE(b/202996544): Intentionally nested to mirror go/glep.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| layer1optionalgroup | [TestNestedGroupExtensionOuter.Layer1OptionalGroup](#objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup) | optional |  |






<a name="objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup"></a>

### TestNestedGroupExtensionOuter.Layer1OptionalGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| layer2repeatedgroup | [TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2RepeatedGroup](#objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup-Layer2RepeatedGroup) | repeated |  |
| layer2anotheroptionalrepeatedgroup | [TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2AnotherOptionalRepeatedGroup](#objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup-Layer2AnotherOptionalRepeatedGroup) | repeated |  |






<a name="objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup-Layer2AnotherOptionalRepeatedGroup"></a>

### TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2AnotherOptionalRepeatedGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| but_why_tho | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestNestedGroupExtensionOuter-Layer1OptionalGroup-Layer2RepeatedGroup"></a>

### TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2RepeatedGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| another_field | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestNestedMessageHasBits"></a>

### TestNestedMessageHasBits
Needed for a Python test.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_nested_message | [TestNestedMessageHasBits.NestedMessage](#objc-protobuf-tests-TestNestedMessageHasBits-NestedMessage) | optional |  |






<a name="objc-protobuf-tests-TestNestedMessageHasBits-NestedMessage"></a>

### TestNestedMessageHasBits.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| nestedmessage_repeated_int32 | [int32](#int32) | repeated |  |
| nestedmessage_repeated_foreignmessage | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | repeated |  |






<a name="objc-protobuf-tests-TestNestedRequiredForeign"></a>

### TestNestedRequiredForeign



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| child | [TestNestedRequiredForeign](#objc-protobuf-tests-TestNestedRequiredForeign) | optional |  |
| payload | [TestRequiredForeign](#objc-protobuf-tests-TestRequiredForeign) | optional |  |
| dummy | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestOneof"></a>

### TestOneof
Test oneofs.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo_int | [int32](#int32) | optional |  |
| foo_string | [string](#string) | optional |  |
| foo_message | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| foogroup | [TestOneof.FooGroup](#objc-protobuf-tests-TestOneof-FooGroup) | optional |  |






<a name="objc-protobuf-tests-TestOneof-FooGroup"></a>

### TestOneof.FooGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| b | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestOneof2"></a>

### TestOneof2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo_int | [int32](#int32) | optional |  |
| foo_string | [string](#string) | optional |  |
| foo_cord | [string](#string) | optional |  |
| foo_string_piece | [string](#string) | optional |  |
| foo_bytes | [bytes](#bytes) | optional |  |
| foo_enum | [TestOneof2.NestedEnum](#objc-protobuf-tests-TestOneof2-NestedEnum) | optional |  |
| foo_message | [TestOneof2.NestedMessage](#objc-protobuf-tests-TestOneof2-NestedMessage) | optional |  |
| foogroup | [TestOneof2.FooGroup](#objc-protobuf-tests-TestOneof2-FooGroup) | optional |  |
| foo_lazy_message | [TestOneof2.NestedMessage](#objc-protobuf-tests-TestOneof2-NestedMessage) | optional |  |
| bar_int | [int32](#int32) | optional |  Default: 5 |
| bar_string | [string](#string) | optional |  Default: STRING |
| bar_cord | [string](#string) | optional |  Default: CORD |
| bar_string_piece | [string](#string) | optional |  Default: SPIECE |
| bar_bytes | [bytes](#bytes) | optional |  Default: BYTES |
| bar_enum | [TestOneof2.NestedEnum](#objc-protobuf-tests-TestOneof2-NestedEnum) | optional |  Default: BAR |
| bar_string_with_empty_default | [string](#string) | optional |  |
| bar_cord_with_empty_default | [string](#string) | optional |  |
| bar_string_piece_with_empty_default | [string](#string) | optional |  |
| bar_bytes_with_empty_default | [bytes](#bytes) | optional |  |
| baz_int | [int32](#int32) | optional |  |
| baz_string | [string](#string) | optional |  Default: BAZ |






<a name="objc-protobuf-tests-TestOneof2-FooGroup"></a>

### TestOneof2.FooGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| b | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestOneof2-NestedMessage"></a>

### TestOneof2.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| moo_int | [int64](#int64) | optional |  |
| corge_int | [int32](#int32) | repeated |  |






<a name="objc-protobuf-tests-TestOneofBackwardsCompatible"></a>

### TestOneofBackwardsCompatible



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo_int | [int32](#int32) | optional |  |
| foo_string | [string](#string) | optional |  |
| foo_message | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| foogroup | [TestOneofBackwardsCompatible.FooGroup](#objc-protobuf-tests-TestOneofBackwardsCompatible-FooGroup) | optional |  |






<a name="objc-protobuf-tests-TestOneofBackwardsCompatible-FooGroup"></a>

### TestOneofBackwardsCompatible.FooGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional |  |
| b | [string](#string) | optional |  |






<a name="objc-protobuf-tests-TestPackedExtensions"></a>

### TestPackedExtensions







<a name="objc-protobuf-tests-TestPackedTypes"></a>

### TestPackedTypes



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| packed_int32 | [int32](#int32) | repeated |  |
| packed_int64 | [int64](#int64) | repeated |  |
| packed_uint32 | [uint32](#uint32) | repeated |  |
| packed_uint64 | [uint64](#uint64) | repeated |  |
| packed_sint32 | [sint32](#sint32) | repeated |  |
| packed_sint64 | [sint64](#sint64) | repeated |  |
| packed_fixed32 | [fixed32](#fixed32) | repeated |  |
| packed_fixed64 | [fixed64](#fixed64) | repeated |  |
| packed_sfixed32 | [sfixed32](#sfixed32) | repeated |  |
| packed_sfixed64 | [sfixed64](#sfixed64) | repeated |  |
| packed_float | [float](#float) | repeated |  |
| packed_double | [double](#double) | repeated |  |
| packed_bool | [bool](#bool) | repeated |  |
| packed_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | repeated |  |






<a name="objc-protobuf-tests-TestParsingMerge"></a>

### TestParsingMerge
Test that if an optional or required message/group field appears multiple
times in the input, they need to be merged.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| required_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | required |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |
| optionalgroup | [TestParsingMerge.OptionalGroup](#objc-protobuf-tests-TestParsingMerge-OptionalGroup) | optional |  |
| repeatedgroup | [TestParsingMerge.RepeatedGroup](#objc-protobuf-tests-TestParsingMerge-RepeatedGroup) | repeated |  |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| optional_ext | TestAllTypes | TestParsingMerge | 1000 |  |
| repeated_ext | TestAllTypes | TestParsingMerge | 1001 |  |




<a name="objc-protobuf-tests-TestParsingMerge-OptionalGroup"></a>

### TestParsingMerge.OptionalGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_group_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator"></a>

### TestParsingMerge.RepeatedFieldsGenerator
RepeatedFieldsGenerator defines matching field types as TestParsingMerge,
except that all fields are repeated. In the tests, we will serialize the
RepeatedFieldsGenerator to bytes, and parse the bytes to TestParsingMerge.
Repeated fields in RepeatedFieldsGenerator are expected to be merged into
the corresponding required/optional fields in TestParsingMerge.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field1 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |
| field2 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |
| field3 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |
| group1 | [TestParsingMerge.RepeatedFieldsGenerator.Group1](#objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator-Group1) | repeated |  |
| group2 | [TestParsingMerge.RepeatedFieldsGenerator.Group2](#objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator-Group2) | repeated |  |
| ext1 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |
| ext2 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator-Group1"></a>

### TestParsingMerge.RepeatedFieldsGenerator.Group1



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field1 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestParsingMerge-RepeatedFieldsGenerator-Group2"></a>

### TestParsingMerge.RepeatedFieldsGenerator.Group2



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field1 | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestParsingMerge-RepeatedGroup"></a>

### TestParsingMerge.RepeatedGroup



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| repeated_group_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |






<a name="objc-protobuf-tests-TestPickleNestedMessage"></a>

### TestPickleNestedMessage
Needed for a Python test.






<a name="objc-protobuf-tests-TestPickleNestedMessage-NestedMessage"></a>

### TestPickleNestedMessage.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bb | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestPickleNestedMessage-NestedMessage-NestedNestedMessage"></a>

### TestPickleNestedMessage.NestedMessage.NestedNestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| cc | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestReallyLargeTagNumber"></a>

### TestReallyLargeTagNumber
Test that really large tag numbers don&#39;t break anything.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | optional | The largest possible tag number is 2^28 - 1, since the wire format uses three bits to communicate wire type. |
| bb | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestRecursiveMessage"></a>

### TestRecursiveMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [TestRecursiveMessage](#objc-protobuf-tests-TestRecursiveMessage) | optional |  |
| i | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestRepeatedScalarDifferentTagSizes"></a>

### TestRepeatedScalarDifferentTagSizes



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| repeated_fixed32 | [fixed32](#fixed32) | repeated | Parsing repeated fixed size values used to fail. This message needs to be used in order to get a tag of the right size; all of the repeated fields in TestAllTypes didn&#39;t trigger the check. |
| repeated_int32 | [int32](#int32) | repeated | Check for a varint type, just for good measure. |
| repeated_fixed64 | [fixed64](#fixed64) | repeated | These have two-byte tags. |
| repeated_int64 | [int64](#int64) | repeated |  |
| repeated_float | [float](#float) | repeated | Three byte tags. |
| repeated_uint64 | [uint64](#uint64) | repeated |  |






<a name="objc-protobuf-tests-TestRequired"></a>

### TestRequired
We have separate messages for testing required fields because it&#39;s
annoying to have to fill in required fields in TestProto in order to
do anything with it.  Note that we don&#39;t need to test every type of
required filed because the code output is basically identical to
optional fields for all types.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| a | [int32](#int32) | required |  |
| dummy2 | [int32](#int32) | optional |  |
| b | [int32](#int32) | required |  |
| dummy4 | [int32](#int32) | optional | Pad the field count to 32 so that we can test that IsInitialized() properly checks multiple elements of has_bits_. |
| dummy5 | [int32](#int32) | optional |  |
| dummy6 | [int32](#int32) | optional |  |
| dummy7 | [int32](#int32) | optional |  |
| dummy8 | [int32](#int32) | optional |  |
| dummy9 | [int32](#int32) | optional |  |
| dummy10 | [int32](#int32) | optional |  |
| dummy11 | [int32](#int32) | optional |  |
| dummy12 | [int32](#int32) | optional |  |
| dummy13 | [int32](#int32) | optional |  |
| dummy14 | [int32](#int32) | optional |  |
| dummy15 | [int32](#int32) | optional |  |
| dummy16 | [int32](#int32) | optional |  |
| dummy17 | [int32](#int32) | optional |  |
| dummy18 | [int32](#int32) | optional |  |
| dummy19 | [int32](#int32) | optional |  |
| dummy20 | [int32](#int32) | optional |  |
| dummy21 | [int32](#int32) | optional |  |
| dummy22 | [int32](#int32) | optional |  |
| dummy23 | [int32](#int32) | optional |  |
| dummy24 | [int32](#int32) | optional |  |
| dummy25 | [int32](#int32) | optional |  |
| dummy26 | [int32](#int32) | optional |  |
| dummy27 | [int32](#int32) | optional |  |
| dummy28 | [int32](#int32) | optional |  |
| dummy29 | [int32](#int32) | optional |  |
| dummy30 | [int32](#int32) | optional |  |
| dummy31 | [int32](#int32) | optional |  |
| dummy32 | [int32](#int32) | optional |  |
| c | [int32](#int32) | required |  |
| optional_foreign | [ForeignMessage](#objc-protobuf-tests-ForeignMessage) | optional | Add an optional child message to make this non-trivial for go/pdlazy. |




| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| single | TestRequired | TestAllExtensions | 1000 |  |
| multi | TestRequired | TestAllExtensions | 1001 |  |




<a name="objc-protobuf-tests-TestRequiredForeign"></a>

### TestRequiredForeign



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_message | [TestRequired](#objc-protobuf-tests-TestRequired) | optional |  |
| repeated_message | [TestRequired](#objc-protobuf-tests-TestRequired) | repeated |  |
| dummy | [int32](#int32) | optional |  |
| optional_lazy_message | [NestedTestAllTypes](#objc-protobuf-tests-NestedTestAllTypes) | optional | Missing required fields must not affect verification of child messages. |






<a name="objc-protobuf-tests-TestRequiredMessage"></a>

### TestRequiredMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_message | [TestRequired](#objc-protobuf-tests-TestRequired) | optional |  |
| repeated_message | [TestRequired](#objc-protobuf-tests-TestRequired) | repeated |  |
| required_message | [TestRequired](#objc-protobuf-tests-TestRequired) | required |  |






<a name="objc-protobuf-tests-TestRequiredOneof"></a>

### TestRequiredOneof



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo_int | [int32](#int32) | optional |  |
| foo_string | [string](#string) | optional |  |
| foo_message | [TestRequiredOneof.NestedMessage](#objc-protobuf-tests-TestRequiredOneof-NestedMessage) | optional |  |






<a name="objc-protobuf-tests-TestRequiredOneof-NestedMessage"></a>

### TestRequiredOneof.NestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| required_double | [double](#double) | required |  |






<a name="objc-protobuf-tests-TestReservedFields"></a>

### TestReservedFields







<a name="objc-protobuf-tests-TestUnpackedExtensions"></a>

### TestUnpackedExtensions







<a name="objc-protobuf-tests-TestUnpackedTypes"></a>

### TestUnpackedTypes
A message with the same fields as TestPackedTypes, but without packing. Used
to test packed &lt;-&gt; unpacked wire compatibility.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| unpacked_int32 | [int32](#int32) | repeated |  |
| unpacked_int64 | [int64](#int64) | repeated |  |
| unpacked_uint32 | [uint32](#uint32) | repeated |  |
| unpacked_uint64 | [uint64](#uint64) | repeated |  |
| unpacked_sint32 | [sint32](#sint32) | repeated |  |
| unpacked_sint64 | [sint64](#sint64) | repeated |  |
| unpacked_fixed32 | [fixed32](#fixed32) | repeated |  |
| unpacked_fixed64 | [fixed64](#fixed64) | repeated |  |
| unpacked_sfixed32 | [sfixed32](#sfixed32) | repeated |  |
| unpacked_sfixed64 | [sfixed64](#sfixed64) | repeated |  |
| unpacked_float | [float](#float) | repeated |  |
| unpacked_double | [double](#double) | repeated |  |
| unpacked_bool | [bool](#bool) | repeated |  |
| unpacked_enum | [ForeignEnum](#objc-protobuf-tests-ForeignEnum) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyBigFieldNumberUint32"></a>

### TestVerifyBigFieldNumberUint32



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_nested | [TestVerifyBigFieldNumberUint32.Nested](#objc-protobuf-tests-TestVerifyBigFieldNumberUint32-Nested) | optional |  |






<a name="objc-protobuf-tests-TestVerifyBigFieldNumberUint32-Nested"></a>

### TestVerifyBigFieldNumberUint32.Nested



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_uint32_5000 | [uint32](#uint32) | optional |  |
| optional_uint32_1000 | [uint32](#uint32) | optional |  |
| optional_uint32_66 | [uint32](#uint32) | optional |  |
| optional_uint32_65 | [uint32](#uint32) | optional |  |
| optional_uint32_1 | [uint32](#uint32) | optional |  |
| optional_uint32_2 | [uint32](#uint32) | optional |  |
| optional_uint32_63 | [uint32](#uint32) | optional |  |
| optional_uint32_64 | [uint32](#uint32) | optional |  |
| optional_nested | [TestVerifyBigFieldNumberUint32.Nested](#objc-protobuf-tests-TestVerifyBigFieldNumberUint32-Nested) | optional |  |
| repeated_nested | [TestVerifyBigFieldNumberUint32.Nested](#objc-protobuf-tests-TestVerifyBigFieldNumberUint32-Nested) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyInt32"></a>

### TestVerifyInt32



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32_1 | [int32](#int32) | optional |  |
| optional_int32_2 | [int32](#int32) | optional |  |
| optional_int32_63 | [int32](#int32) | optional |  |
| optional_int32_64 | [int32](#int32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyInt32BigFieldNumber"></a>

### TestVerifyInt32BigFieldNumber



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32_1000 | [int32](#int32) | optional |  |
| optional_int32_65 | [int32](#int32) | optional |  |
| optional_int32_1 | [int32](#int32) | optional |  |
| optional_int32_2 | [int32](#int32) | optional |  |
| optional_int32_63 | [int32](#int32) | optional |  |
| optional_int32_64 | [int32](#int32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyInt32Simple"></a>

### TestVerifyInt32Simple



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32_1 | [int32](#int32) | optional |  |
| optional_int32_2 | [int32](#int32) | optional |  |
| optional_int32_63 | [int32](#int32) | optional |  |
| optional_int32_64 | [int32](#int32) | optional |  |






<a name="objc-protobuf-tests-TestVerifyMostlyInt32"></a>

### TestVerifyMostlyInt32



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int64_30 | [int64](#int64) | optional |  |
| optional_int32_1 | [int32](#int32) | optional |  |
| optional_int32_2 | [int32](#int32) | optional |  |
| optional_int32_3 | [int32](#int32) | optional |  |
| optional_int32_4 | [int32](#int32) | optional |  |
| optional_int32_63 | [int32](#int32) | optional |  |
| optional_int32_64 | [int32](#int32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyMostlyInt32BigFieldNumber"></a>

### TestVerifyMostlyInt32BigFieldNumber



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int64_30 | [int64](#int64) | optional |  |
| optional_int32_300 | [int32](#int32) | optional |  |
| optional_int32_1 | [int32](#int32) | optional |  |
| optional_int32_2 | [int32](#int32) | optional |  |
| optional_int32_3 | [int32](#int32) | optional |  |
| optional_int32_4 | [int32](#int32) | optional |  |
| optional_int32_63 | [int32](#int32) | optional |  |
| optional_int32_64 | [int32](#int32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyOneInt32BigFieldNumber"></a>

### TestVerifyOneInt32BigFieldNumber



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_int32_65 | [int32](#int32) | optional |  |
| optional_int64_1 | [int64](#int64) | optional |  |
| optional_int64_2 | [int64](#int64) | optional |  |
| optional_int64_63 | [int64](#int64) | optional |  |
| optional_int64_64 | [int64](#int64) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyOneUint32"></a>

### TestVerifyOneUint32



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_uint32_1 | [uint32](#uint32) | optional |  |
| optional_int32_2 | [int32](#int32) | optional |  |
| optional_int32_63 | [int32](#int32) | optional |  |
| optional_int32_64 | [int32](#int32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyUint32"></a>

### TestVerifyUint32



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_uint32_1 | [uint32](#uint32) | optional |  |
| optional_uint32_2 | [uint32](#uint32) | optional |  |
| optional_uint32_63 | [uint32](#uint32) | optional |  |
| optional_uint32_64 | [uint32](#uint32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyUint32BigFieldNumber"></a>

### TestVerifyUint32BigFieldNumber



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_uint32_1000 | [uint32](#uint32) | optional |  |
| optional_uint32_65 | [uint32](#uint32) | optional |  |
| optional_uint32_1 | [uint32](#uint32) | optional |  |
| optional_uint32_2 | [uint32](#uint32) | optional |  |
| optional_uint32_63 | [uint32](#uint32) | optional |  |
| optional_uint32_64 | [uint32](#uint32) | optional |  |
| optional_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | optional |  |
| repeated_all_types | [TestAllTypes](#objc-protobuf-tests-TestAllTypes) | repeated |  |






<a name="objc-protobuf-tests-TestVerifyUint32Simple"></a>

### TestVerifyUint32Simple



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_uint32_1 | [uint32](#uint32) | optional |  |
| optional_uint32_2 | [uint32](#uint32) | optional |  |
| optional_uint32_63 | [uint32](#uint32) | optional |  |
| optional_uint32_64 | [uint32](#uint32) | optional |  |






<a name="objc-protobuf-tests-Uint32Message"></a>

### Uint32Message



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [uint32](#uint32) | optional |  |






<a name="objc-protobuf-tests-Uint64Message"></a>

### Uint64Message



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| data | [uint64](#uint64) | optional |  |





 


<a name="objc-protobuf-tests-EnumParseTester-Arbitrary"></a>

### EnumParseTester.Arbitrary


| Name | Number | Description |
| ---- | ------ | ----------- |
| ARBITRARY_DEFAULT | -123123 |  |
| ARBITRARY_1 | -123 |  |
| ARBITRARY_2 | 213 |  |
| ARBITRARY_3 | 213213 |  |
| ARBITRARY_MIN | -2147483648 |  |
| ARBITRARY_MAX | 2147483647 |  |



<a name="objc-protobuf-tests-EnumParseTester-SeqLarge"></a>

### EnumParseTester.SeqLarge


| Name | Number | Description |
| ---- | ------ | ----------- |
| SEQ_LARGE_DEFAULT | -1 |  |
| SEQ_LARGE_0 | 0 |  |
| SEQ_LARGE_1 | 1 |  |
| SEQ_LARGE_2 | 2 |  |
| SEQ_LARGE_3 | 3 |  |
| SEQ_LARGE_4 | 4 |  |
| SEQ_LARGE_5 | 5 |  |
| SEQ_LARGE_6 | 6 |  |
| SEQ_LARGE_7 | 7 |  |
| SEQ_LARGE_8 | 8 |  |
| SEQ_LARGE_9 | 9 |  |
| SEQ_LARGE_10 | 10 |  |
| SEQ_LARGE_11 | 11 |  |
| SEQ_LARGE_12 | 12 |  |
| SEQ_LARGE_13 | 13 |  |
| SEQ_LARGE_14 | 14 |  |
| SEQ_LARGE_15 | 15 |  |
| SEQ_LARGE_16 | 16 |  |
| SEQ_LARGE_17 | 17 |  |
| SEQ_LARGE_18 | 18 |  |
| SEQ_LARGE_19 | 19 |  |
| SEQ_LARGE_20 | 20 |  |
| SEQ_LARGE_21 | 21 |  |
| SEQ_LARGE_22 | 22 |  |
| SEQ_LARGE_23 | 23 |  |
| SEQ_LARGE_24 | 24 |  |
| SEQ_LARGE_25 | 25 |  |
| SEQ_LARGE_26 | 26 |  |
| SEQ_LARGE_27 | 27 |  |
| SEQ_LARGE_28 | 28 |  |
| SEQ_LARGE_29 | 29 |  |
| SEQ_LARGE_30 | 30 |  |
| SEQ_LARGE_31 | 31 |  |
| SEQ_LARGE_32 | 32 |  |
| SEQ_LARGE_33 | 33 |  |



<a name="objc-protobuf-tests-EnumParseTester-SeqSmall0"></a>

### EnumParseTester.SeqSmall0


| Name | Number | Description |
| ---- | ------ | ----------- |
| SEQ_SMALL_0_DEFAULT | 0 |  |
| SEQ_SMALL_0_1 | 1 |  |
| SEQ_SMALL_0_2 | 2 |  |



<a name="objc-protobuf-tests-EnumParseTester-SeqSmall1"></a>

### EnumParseTester.SeqSmall1


| Name | Number | Description |
| ---- | ------ | ----------- |
| SEQ_SMALL_1_DEFAULT | 1 |  |
| SEQ_SMALL_1_2 | 2 |  |
| SEQ_SMALL_1_3 | 3 |  |



<a name="objc-protobuf-tests-ForeignEnum"></a>

### ForeignEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOREIGN_FOO | 4 |  |
| FOREIGN_BAR | 5 |  |
| FOREIGN_BAZ | 6 |  |



<a name="objc-protobuf-tests-TestAllTypes-NestedEnum"></a>

### TestAllTypes.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 1 |  |
| BAR | 2 |  |
| BAZ | 3 |  |
| NEG | -1 | Intentionally negative. |



<a name="objc-protobuf-tests-TestDynamicExtensions-DynamicEnumType"></a>

### TestDynamicExtensions.DynamicEnumType


| Name | Number | Description |
| ---- | ------ | ----------- |
| DYNAMIC_FOO | 2200 |  |
| DYNAMIC_BAR | 2201 |  |
| DYNAMIC_BAZ | 2202 |  |



<a name="objc-protobuf-tests-TestEnumWithDupValue"></a>

### TestEnumWithDupValue
Test an enum that has multiple values with the same number.

| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO1 | 1 |  |
| BAR1 | 2 |  |
| BAZ | 3 |  |
| FOO2 | 1 |  |
| BAR2 | 2 |  |



<a name="objc-protobuf-tests-TestOneof2-NestedEnum"></a>

### TestOneof2.NestedEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| FOO | 1 |  |
| BAR | 2 |  |
| BAZ | 3 |  |



<a name="objc-protobuf-tests-TestReservedEnumFields"></a>

### TestReservedEnumFields


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 |  |



<a name="objc-protobuf-tests-TestSparseEnum"></a>

### TestSparseEnum
Test an enum with large, unordered values.

| Name | Number | Description |
| ---- | ------ | ----------- |
| SPARSE_A | 123 |  |
| SPARSE_B | 62374 |  |
| SPARSE_C | 12589234 |  |
| SPARSE_D | -15 |  |
| SPARSE_E | -53452 |  |
| SPARSE_F | 0 |  |
| SPARSE_G | 2 |  |



<a name="objc-protobuf-tests-VeryLargeEnum"></a>

### VeryLargeEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ENUM_LABEL_DEFAULT | 0 |  |
| ENUM_LABEL_1 | 1 |  |
| ENUM_LABEL_2 | 2 |  |
| ENUM_LABEL_3 | 3 |  |
| ENUM_LABEL_4 | 4 |  |
| ENUM_LABEL_5 | 5 |  |
| ENUM_LABEL_6 | 6 |  |
| ENUM_LABEL_7 | 7 |  |
| ENUM_LABEL_8 | 8 |  |
| ENUM_LABEL_9 | 9 |  |
| ENUM_LABEL_10 | 10 |  |
| ENUM_LABEL_11 | 11 |  |
| ENUM_LABEL_12 | 12 |  |
| ENUM_LABEL_13 | 13 |  |
| ENUM_LABEL_14 | 14 |  |
| ENUM_LABEL_15 | 15 |  |
| ENUM_LABEL_16 | 16 |  |
| ENUM_LABEL_17 | 17 |  |
| ENUM_LABEL_18 | 18 |  |
| ENUM_LABEL_19 | 19 |  |
| ENUM_LABEL_20 | 20 |  |
| ENUM_LABEL_21 | 21 |  |
| ENUM_LABEL_22 | 22 |  |
| ENUM_LABEL_23 | 23 |  |
| ENUM_LABEL_24 | 24 |  |
| ENUM_LABEL_25 | 25 |  |
| ENUM_LABEL_26 | 26 |  |
| ENUM_LABEL_27 | 27 |  |
| ENUM_LABEL_28 | 28 |  |
| ENUM_LABEL_29 | 29 |  |
| ENUM_LABEL_30 | 30 |  |
| ENUM_LABEL_31 | 31 |  |
| ENUM_LABEL_32 | 32 |  |
| ENUM_LABEL_33 | 33 |  |
| ENUM_LABEL_34 | 34 |  |
| ENUM_LABEL_35 | 35 |  |
| ENUM_LABEL_36 | 36 |  |
| ENUM_LABEL_37 | 37 |  |
| ENUM_LABEL_38 | 38 |  |
| ENUM_LABEL_39 | 39 |  |
| ENUM_LABEL_40 | 40 |  |
| ENUM_LABEL_41 | 41 |  |
| ENUM_LABEL_42 | 42 |  |
| ENUM_LABEL_43 | 43 |  |
| ENUM_LABEL_44 | 44 |  |
| ENUM_LABEL_45 | 45 |  |
| ENUM_LABEL_46 | 46 |  |
| ENUM_LABEL_47 | 47 |  |
| ENUM_LABEL_48 | 48 |  |
| ENUM_LABEL_49 | 49 |  |
| ENUM_LABEL_50 | 50 |  |
| ENUM_LABEL_51 | 51 |  |
| ENUM_LABEL_52 | 52 |  |
| ENUM_LABEL_53 | 53 |  |
| ENUM_LABEL_54 | 54 |  |
| ENUM_LABEL_55 | 55 |  |
| ENUM_LABEL_56 | 56 |  |
| ENUM_LABEL_57 | 57 |  |
| ENUM_LABEL_58 | 58 |  |
| ENUM_LABEL_59 | 59 |  |
| ENUM_LABEL_60 | 60 |  |
| ENUM_LABEL_61 | 61 |  |
| ENUM_LABEL_62 | 62 |  |
| ENUM_LABEL_63 | 63 |  |
| ENUM_LABEL_64 | 64 |  |
| ENUM_LABEL_65 | 65 |  |
| ENUM_LABEL_66 | 66 |  |
| ENUM_LABEL_67 | 67 |  |
| ENUM_LABEL_68 | 68 |  |
| ENUM_LABEL_69 | 69 |  |
| ENUM_LABEL_70 | 70 |  |
| ENUM_LABEL_71 | 71 |  |
| ENUM_LABEL_72 | 72 |  |
| ENUM_LABEL_73 | 73 |  |
| ENUM_LABEL_74 | 74 |  |
| ENUM_LABEL_75 | 75 |  |
| ENUM_LABEL_76 | 76 |  |
| ENUM_LABEL_77 | 77 |  |
| ENUM_LABEL_78 | 78 |  |
| ENUM_LABEL_79 | 79 |  |
| ENUM_LABEL_80 | 80 |  |
| ENUM_LABEL_81 | 81 |  |
| ENUM_LABEL_82 | 82 |  |
| ENUM_LABEL_83 | 83 |  |
| ENUM_LABEL_84 | 84 |  |
| ENUM_LABEL_85 | 85 |  |
| ENUM_LABEL_86 | 86 |  |
| ENUM_LABEL_87 | 87 |  |
| ENUM_LABEL_88 | 88 |  |
| ENUM_LABEL_89 | 89 |  |
| ENUM_LABEL_90 | 90 |  |
| ENUM_LABEL_91 | 91 |  |
| ENUM_LABEL_92 | 92 |  |
| ENUM_LABEL_93 | 93 |  |
| ENUM_LABEL_94 | 94 |  |
| ENUM_LABEL_95 | 95 |  |
| ENUM_LABEL_96 | 96 |  |
| ENUM_LABEL_97 | 97 |  |
| ENUM_LABEL_98 | 98 |  |
| ENUM_LABEL_99 | 99 |  |
| ENUM_LABEL_100 | 100 |  |


 


<a name="objectivec_Tests_unittest-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| inner | TestNestedGroupExtensionInnerExtension | TestNestedGroupExtensionOuter.Layer1OptionalGroup.Layer2RepeatedGroup | 3 |  |
| default_bool_extension | bool | TestAllExtensions | 73 |  Default: `true` |
| default_bytes_extension | bytes | TestAllExtensions | 75 |  Default: `world` |
| default_cord_extension | string | TestAllExtensions | 85 |  Default: `123` |
| default_double_extension | double | TestAllExtensions | 72 |  Default: `52000` |
| default_fixed32_extension | fixed32 | TestAllExtensions | 67 |  Default: `47` |
| default_fixed64_extension | fixed64 | TestAllExtensions | 68 |  Default: `48` |
| default_float_extension | float | TestAllExtensions | 71 |  Default: `51.5` |
| default_foreign_enum_extension | ForeignEnum | TestAllExtensions | 82 |  Default: `FOREIGN_BAR` |
| default_import_enum_extension | import.Enum | TestAllExtensions | 83 |  Default: `IMPORT_BAR` |
| default_int32_extension | int32 | TestAllExtensions | 61 | Singular with defaults Default: `41` |
| default_int64_extension | int64 | TestAllExtensions | 62 |  Default: `42` |
| default_nested_enum_extension | TestAllTypes.NestedEnum | TestAllExtensions | 81 |  Default: `BAR` |
| default_sfixed32_extension | sfixed32 | TestAllExtensions | 69 |  Default: `49` |
| default_sfixed64_extension | sfixed64 | TestAllExtensions | 70 |  Default: `-50` |
| default_sint32_extension | sint32 | TestAllExtensions | 65 |  Default: `-45` |
| default_sint64_extension | sint64 | TestAllExtensions | 66 |  Default: `46` |
| default_string_extension | string | TestAllExtensions | 74 |  Default: `hello` |
| default_string_piece_extension | string | TestAllExtensions | 84 |  Default: `abc` |
| default_uint32_extension | uint32 | TestAllExtensions | 63 |  Default: `43` |
| default_uint64_extension | uint64 | TestAllExtensions | 64 |  Default: `44` |
| oneof_bytes_extension | bytes | TestAllExtensions | 114 |  |
| oneof_nested_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 112 |  |
| oneof_string_extension | string | TestAllExtensions | 113 |  |
| oneof_uint32_extension | uint32 | TestAllExtensions | 111 | For oneof test |
| optional_bool_extension | bool | TestAllExtensions | 13 |  |
| optional_bytes_extension | bytes | TestAllExtensions | 15 |  |
| optional_cord_extension | string | TestAllExtensions | 25 |  |
| optional_double_extension | double | TestAllExtensions | 12 |  |
| optional_fixed32_extension | fixed32 | TestAllExtensions | 7 |  |
| optional_fixed64_extension | fixed64 | TestAllExtensions | 8 |  |
| optional_float_extension | float | TestAllExtensions | 11 |  |
| optional_foreign_enum_extension | ForeignEnum | TestAllExtensions | 22 |  |
| optional_foreign_message_extension | ForeignMessage | TestAllExtensions | 19 |  |
| optional_import_enum_extension | import.Enum | TestAllExtensions | 23 |  |
| optional_import_message_extension | import.Message | TestAllExtensions | 20 |  |
| optional_int32_extension | int32 | TestAllExtensions | 1 | Singular |
| optional_int64_extension | int64 | TestAllExtensions | 2 |  |
| optional_lazy_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 27 |  |
| optional_nested_enum_extension | TestAllTypes.NestedEnum | TestAllExtensions | 21 |  |
| optional_nested_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 18 |  |
| optional_public_import_message_extension | public_import.Message | TestAllExtensions | 26 |  |
| optional_sfixed32_extension | sfixed32 | TestAllExtensions | 9 |  |
| optional_sfixed64_extension | sfixed64 | TestAllExtensions | 10 |  |
| optional_sint32_extension | sint32 | TestAllExtensions | 5 |  |
| optional_sint64_extension | sint64 | TestAllExtensions | 6 |  |
| optional_string_extension | string | TestAllExtensions | 14 |  |
| optional_string_piece_extension | string | TestAllExtensions | 24 |  |
| optional_uint32_extension | uint32 | TestAllExtensions | 3 |  |
| optional_uint64_extension | uint64 | TestAllExtensions | 4 |  |
| optional_unverified_lazy_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 28 |  |
| optionalgroup_extension | OptionalGroup_extension | TestAllExtensions | 16 |  |
| repeated_bool_extension | bool | TestAllExtensions | 43 |  |
| repeated_bytes_extension | bytes | TestAllExtensions | 45 |  |
| repeated_cord_extension | string | TestAllExtensions | 55 |  |
| repeated_double_extension | double | TestAllExtensions | 42 |  |
| repeated_fixed32_extension | fixed32 | TestAllExtensions | 37 |  |
| repeated_fixed64_extension | fixed64 | TestAllExtensions | 38 |  |
| repeated_float_extension | float | TestAllExtensions | 41 |  |
| repeated_foreign_enum_extension | ForeignEnum | TestAllExtensions | 52 |  |
| repeated_foreign_message_extension | ForeignMessage | TestAllExtensions | 49 |  |
| repeated_import_enum_extension | import.Enum | TestAllExtensions | 53 |  |
| repeated_import_message_extension | import.Message | TestAllExtensions | 50 |  |
| repeated_int32_extension | int32 | TestAllExtensions | 31 | Repeated |
| repeated_int64_extension | int64 | TestAllExtensions | 32 |  |
| repeated_lazy_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 57 |  |
| repeated_nested_enum_extension | TestAllTypes.NestedEnum | TestAllExtensions | 51 |  |
| repeated_nested_message_extension | TestAllTypes.NestedMessage | TestAllExtensions | 48 |  |
| repeated_sfixed32_extension | sfixed32 | TestAllExtensions | 39 |  |
| repeated_sfixed64_extension | sfixed64 | TestAllExtensions | 40 |  |
| repeated_sint32_extension | sint32 | TestAllExtensions | 35 |  |
| repeated_sint64_extension | sint64 | TestAllExtensions | 36 |  |
| repeated_string_extension | string | TestAllExtensions | 44 |  |
| repeated_string_piece_extension | string | TestAllExtensions | 54 |  |
| repeated_uint32_extension | uint32 | TestAllExtensions | 33 |  |
| repeated_uint64_extension | uint64 | TestAllExtensions | 34 |  |
| repeatedgroup_extension | RepeatedGroup_extension | TestAllExtensions | 46 |  |
| test_extension_inside_table_extension | int32 | TestExtensionInsideTable | 5 |  |
| my_extension_int | int32 | TestFieldOrderings | 5 |  |
| my_extension_string | string | TestFieldOrderings | 50 |  |
| test_all_types | TestAllTypes | TestHugeFieldNumbers | 536860000 |  |
| packed_bool_extension | bool | TestPackedExtensions | 102 |  |
| packed_double_extension | double | TestPackedExtensions | 101 |  |
| packed_enum_extension | ForeignEnum | TestPackedExtensions | 103 |  |
| packed_fixed32_extension | fixed32 | TestPackedExtensions | 96 |  |
| packed_fixed64_extension | fixed64 | TestPackedExtensions | 97 |  |
| packed_float_extension | float | TestPackedExtensions | 100 |  |
| packed_int32_extension | int32 | TestPackedExtensions | 90 |  |
| packed_int64_extension | int64 | TestPackedExtensions | 91 |  |
| packed_sfixed32_extension | sfixed32 | TestPackedExtensions | 98 |  |
| packed_sfixed64_extension | sfixed64 | TestPackedExtensions | 99 |  |
| packed_sint32_extension | sint32 | TestPackedExtensions | 94 |  |
| packed_sint64_extension | sint64 | TestPackedExtensions | 95 |  |
| packed_uint32_extension | uint32 | TestPackedExtensions | 92 |  |
| packed_uint64_extension | uint64 | TestPackedExtensions | 93 |  |
| unpacked_bool_extension | bool | TestUnpackedExtensions | 102 |  |
| unpacked_double_extension | double | TestUnpackedExtensions | 101 |  |
| unpacked_enum_extension | ForeignEnum | TestUnpackedExtensions | 103 |  |
| unpacked_fixed32_extension | fixed32 | TestUnpackedExtensions | 96 |  |
| unpacked_fixed64_extension | fixed64 | TestUnpackedExtensions | 97 |  |
| unpacked_float_extension | float | TestUnpackedExtensions | 100 |  |
| unpacked_int32_extension | int32 | TestUnpackedExtensions | 90 |  |
| unpacked_int64_extension | int64 | TestUnpackedExtensions | 91 |  |
| unpacked_sfixed32_extension | sfixed32 | TestUnpackedExtensions | 98 |  |
| unpacked_sfixed64_extension | sfixed64 | TestUnpackedExtensions | 99 |  |
| unpacked_sint32_extension | sint32 | TestUnpackedExtensions | 94 |  |
| unpacked_sint64_extension | sint64 | TestUnpackedExtensions | 95 |  |
| unpacked_uint32_extension | uint32 | TestUnpackedExtensions | 92 |  |
| unpacked_uint64_extension | uint64 | TestUnpackedExtensions | 93 |  |

 


<a name="objc-protobuf-tests-TestService"></a>

### TestService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| Foo | [FooRequest](#objc-protobuf-tests-FooRequest) | [FooResponse](#objc-protobuf-tests-FooResponse) |  |
| Bar | [BarRequest](#objc-protobuf-tests-BarRequest) | [BarResponse](#objc-protobuf-tests-BarResponse) |  |

 



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

