# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/core/src/test/proto/com/google/protobuf/proto2_message_lite.proto](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto)
    - [FieldGroup49](#protobuf-experimental-lite-FieldGroup49)
    - [FieldGroupList51](#protobuf-experimental-lite-FieldGroupList51)
    - [Proto2EmptyLite](#protobuf-experimental-lite-Proto2EmptyLite)
    - [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite)
    - [Proto2MessageLite.FieldGroup49](#protobuf-experimental-lite-Proto2MessageLite-FieldGroup49)
    - [Proto2MessageLite.FieldGroup69](#protobuf-experimental-lite-Proto2MessageLite-FieldGroup69)
    - [Proto2MessageLite.FieldGroupList51](#protobuf-experimental-lite-Proto2MessageLite-FieldGroupList51)
    - [Proto2MessageLite.FieldRequiredGroup88](#protobuf-experimental-lite-Proto2MessageLite-FieldRequiredGroup88)
    - [Proto2MessageLite.RequiredNestedMessage](#protobuf-experimental-lite-Proto2MessageLite-RequiredNestedMessage)
    - [Proto2MessageLiteWithExtensions](#protobuf-experimental-lite-Proto2MessageLiteWithExtensions)
    - [Proto2MessageLiteWithMaps](#protobuf-experimental-lite-Proto2MessageLiteWithMaps)
    - [Proto2MessageLiteWithMaps.FieldMapBoolBool1Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolBool1Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolBytes2Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolBytes2Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolDouble3Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolDouble3Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolEnum4Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolEnum4Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolFixed325Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFixed325Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolFixed646Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFixed646Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolFloat7Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFloat7Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolInt328Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolInt328Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolInt649Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolInt649Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolMessage10Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolMessage10Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolSfixed3211Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSfixed3211Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolSfixed6412Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSfixed6412Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolSint3213Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSint3213Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolSint6414Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSint6414Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolString15Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolString15Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolUint3216Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolUint3216Entry)
    - [Proto2MessageLiteWithMaps.FieldMapBoolUint6417Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolUint6417Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Bool18Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Bool18Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Bytes19Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Bytes19Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Double20Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Double20Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Enum21Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Enum21Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Fixed3222Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Fixed3222Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Fixed6423Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Fixed6423Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Float24Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Float24Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Int3225Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Int3225Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Int6426Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Int6426Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Message27Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Message27Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Sfixed3228Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sfixed3228Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Sfixed6429Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sfixed6429Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Sint3230Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sint3230Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Sint6431Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sint6431Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32String32Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32String32Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Uint3233Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Uint3233Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed32Uint6434Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Uint6434Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Bool35Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Bool35Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Bytes36Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Bytes36Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Double37Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Double37Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Enum38Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Enum38Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Fixed3239Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Fixed3239Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Fixed6440Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Fixed6440Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Float41Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Float41Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Int3242Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Int3242Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Int6443Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Int6443Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Message44Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Message44Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Sfixed3245Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sfixed3245Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Sfixed6446Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sfixed6446Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Sint3247Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sint3247Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Sint6448Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sint6448Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64String49Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64String49Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Uint3250Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Uint3250Entry)
    - [Proto2MessageLiteWithMaps.FieldMapFixed64Uint6451Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Uint6451Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Bool52Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Bool52Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Bytes53Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Bytes53Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Double54Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Double54Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Enum55Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Enum55Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Fixed3256Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Fixed3256Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Fixed6457Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Fixed6457Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Float58Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Float58Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Int3259Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Int3259Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Int6460Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Int6460Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Message61Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Message61Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Sfixed3262Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sfixed3262Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Sfixed6463Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sfixed6463Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Sint3264Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sint3264Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Sint6465Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sint6465Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32String66Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32String66Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Uint3267Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Uint3267Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt32Uint6468Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Uint6468Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Bool69Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Bool69Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Bytes70Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Bytes70Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Double71Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Double71Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Enum72Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Enum72Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Fixed3273Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Fixed3273Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Fixed6474Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Fixed6474Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Float75Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Float75Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Int3276Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Int3276Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Int6477Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Int6477Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Message78Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Message78Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Sfixed3279Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sfixed3279Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Sfixed6480Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sfixed6480Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Sint3281Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sint3281Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Sint6482Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sint6482Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64String83Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64String83Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Uint3284Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Uint3284Entry)
    - [Proto2MessageLiteWithMaps.FieldMapInt64Uint6485Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Uint6485Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Bool86Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Bool86Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Bytes87Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Bytes87Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Double88Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Double88Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Enum89Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Enum89Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Fixed3290Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Fixed3290Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Fixed6491Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Fixed6491Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Float92Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Float92Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Int3293Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Int3293Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Int6494Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Int6494Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Message95Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Message95Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Sfixed3296Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sfixed3296Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Sfixed6497Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sfixed6497Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Sint3298Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sint3298Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Sint6499Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sint6499Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32String100Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32String100Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Uint32101Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Uint32101Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed32Uint64102Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Uint64102Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Bool103Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Bool103Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Bytes104Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Bytes104Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Double105Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Double105Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Enum106Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Enum106Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Fixed32107Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Fixed32107Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Fixed64108Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Fixed64108Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Float109Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Float109Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Int32110Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Int32110Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Int64111Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Int64111Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Message112Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Message112Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Sfixed32113Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sfixed32113Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Sfixed64114Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sfixed64114Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Sint32115Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sint32115Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Sint64116Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sint64116Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64String117Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64String117Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Uint32118Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Uint32118Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSfixed64Uint64119Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Uint64119Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Bool120Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Bool120Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Bytes121Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Bytes121Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Double122Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Double122Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Enum123Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Enum123Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Fixed32124Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Fixed32124Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Fixed64125Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Fixed64125Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Float126Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Float126Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Int32127Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Int32127Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Int64128Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Int64128Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Message129Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Message129Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Sfixed32130Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sfixed32130Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Sfixed64131Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sfixed64131Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Sint32132Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sint32132Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Sint64133Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sint64133Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32String134Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32String134Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Uint32135Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Uint32135Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint32Uint64136Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Uint64136Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Bool137Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Bool137Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Bytes138Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Bytes138Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Double139Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Double139Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Enum140Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Enum140Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Fixed32141Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Fixed32141Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Fixed64142Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Fixed64142Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Float143Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Float143Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Int32144Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Int32144Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Int64145Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Int64145Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Message146Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Message146Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Sfixed32147Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sfixed32147Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Sfixed64148Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sfixed64148Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Sint32149Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sint32149Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Sint64150Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sint64150Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64String151Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64String151Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Uint32152Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Uint32152Entry)
    - [Proto2MessageLiteWithMaps.FieldMapSint64Uint64153Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Uint64153Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringBool154Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringBool154Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringBytes155Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringBytes155Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringDouble156Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringDouble156Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringEnum157Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringEnum157Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringFixed32158Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFixed32158Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringFixed64159Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFixed64159Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringFloat160Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFloat160Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringInt32161Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringInt32161Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringInt64162Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringInt64162Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringMessage163Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringMessage163Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringSfixed32164Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSfixed32164Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringSfixed64165Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSfixed64165Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringSint32166Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSint32166Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringSint64167Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSint64167Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringString168Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringString168Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringUint32169Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringUint32169Entry)
    - [Proto2MessageLiteWithMaps.FieldMapStringUint64170Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringUint64170Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Bool171Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Bool171Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Bytes172Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Bytes172Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Double173Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Double173Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Enum174Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Enum174Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Fixed32175Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Fixed32175Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Fixed64176Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Fixed64176Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Float177Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Float177Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Int32178Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Int32178Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Int64179Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Int64179Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Message180Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Message180Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Sfixed32181Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sfixed32181Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Sfixed64182Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sfixed64182Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Sint32183Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sint32183Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Sint64184Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sint64184Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32String185Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32String185Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Uint32186Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Uint32186Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint32Uint64187Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Uint64187Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Bool188Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Bool188Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Bytes189Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Bytes189Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Double190Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Double190Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Enum191Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Enum191Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Fixed32192Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Fixed32192Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Fixed64193Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Fixed64193Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Float194Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Float194Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Int32195Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Int32195Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Int64196Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Int64196Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Message197Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Message197Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Sfixed32198Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sfixed32198Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Sfixed64199Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sfixed64199Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Sint32200Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sint32200Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Sint64201Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sint64201Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64String202Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64String202Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Uint32203Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Uint32203Entry)
    - [Proto2MessageLiteWithMaps.FieldMapUint64Uint64204Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Uint64204Entry)
  
    - [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum)
  
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/core/src/test/proto/com/google/protobuf/proto2_message_lite.proto
LINT: ALLOW_GROUPS


<a name="protobuf-experimental-lite-FieldGroup49"></a>

### FieldGroup49



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_50 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-FieldGroupList51"></a>

### FieldGroupList51



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_52 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2EmptyLite"></a>

### Proto2EmptyLite







<a name="protobuf-experimental-lite-Proto2MessageLite"></a>

### Proto2MessageLite



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_double_1 | [double](#double) | optional |  |
| field_float_2 | [float](#float) | optional |  |
| field_int64_3 | [int64](#int64) | optional |  |
| field_uint64_4 | [uint64](#uint64) | optional |  |
| field_int32_5 | [int32](#int32) | optional |  |
| field_fixed64_6 | [fixed64](#fixed64) | optional |  |
| field_fixed32_7 | [fixed32](#fixed32) | optional |  |
| field_bool_8 | [bool](#bool) | optional |  |
| field_string_9 | [string](#string) | optional |  |
| field_message_10 | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |
| field_bytes_11 | [bytes](#bytes) | optional |  |
| field_uint32_12 | [uint32](#uint32) | optional |  |
| field_enum_13 | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |
| field_sfixed32_14 | [sfixed32](#sfixed32) | optional |  |
| field_sfixed64_15 | [sfixed64](#sfixed64) | optional |  |
| field_sint32_16 | [sint32](#sint32) | optional |  |
| field_sint64_17 | [sint64](#sint64) | optional |  |
| field_double_list_18 | [double](#double) | repeated |  |
| field_float_list_19 | [float](#float) | repeated |  |
| field_int64_list_20 | [int64](#int64) | repeated |  |
| field_uint64_list_21 | [uint64](#uint64) | repeated |  |
| field_int32_list_22 | [int32](#int32) | repeated |  |
| field_fixed64_list_23 | [fixed64](#fixed64) | repeated |  |
| field_fixed32_list_24 | [fixed32](#fixed32) | repeated |  |
| field_bool_list_25 | [bool](#bool) | repeated |  |
| field_string_list_26 | [string](#string) | repeated |  |
| field_message_list_27 | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | repeated |  |
| field_bytes_list_28 | [bytes](#bytes) | repeated |  |
| field_uint32_list_29 | [uint32](#uint32) | repeated |  |
| field_enum_list_30 | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | repeated |  |
| field_sfixed32_list_31 | [sfixed32](#sfixed32) | repeated |  |
| field_sfixed64_list_32 | [sfixed64](#sfixed64) | repeated |  |
| field_sint32_list_33 | [sint32](#sint32) | repeated |  |
| field_sint64_list_34 | [sint64](#sint64) | repeated |  |
| field_double_list_packed_35 | [double](#double) | repeated |  |
| field_float_list_packed_36 | [float](#float) | repeated |  |
| field_int64_list_packed_37 | [int64](#int64) | repeated |  |
| field_uint64_list_packed_38 | [uint64](#uint64) | repeated |  |
| field_int32_list_packed_39 | [int32](#int32) | repeated |  |
| field_fixed64_list_packed_40 | [fixed64](#fixed64) | repeated |  |
| field_fixed32_list_packed_41 | [fixed32](#fixed32) | repeated |  |
| field_bool_list_packed_42 | [bool](#bool) | repeated |  |
| field_uint32_list_packed_43 | [uint32](#uint32) | repeated |  |
| field_enum_list_packed_44 | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | repeated |  |
| field_sfixed32_list_packed_45 | [sfixed32](#sfixed32) | repeated |  |
| field_sfixed64_list_packed_46 | [sfixed64](#sfixed64) | repeated |  |
| field_sint32_list_packed_47 | [sint32](#sint32) | repeated |  |
| field_sint64_list_packed_48 | [sint64](#sint64) | repeated |  |
| fieldgroup49 | [Proto2MessageLite.FieldGroup49](#protobuf-experimental-lite-Proto2MessageLite-FieldGroup49) | optional |  |
| fieldgrouplist51 | [Proto2MessageLite.FieldGroupList51](#protobuf-experimental-lite-Proto2MessageLite-FieldGroupList51) | repeated |  |
| field_double_53 | [double](#double) | optional |  |
| field_float_54 | [float](#float) | optional |  |
| field_int64_55 | [int64](#int64) | optional |  |
| field_uint64_56 | [uint64](#uint64) | optional |  |
| field_int32_57 | [int32](#int32) | optional |  |
| field_fixed64_58 | [fixed64](#fixed64) | optional |  |
| field_fixed32_59 | [fixed32](#fixed32) | optional |  |
| field_bool_60 | [bool](#bool) | optional |  |
| field_string_61 | [string](#string) | optional |  |
| field_message_62 | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |
| field_bytes_63 | [bytes](#bytes) | optional |  |
| field_uint32_64 | [uint32](#uint32) | optional |  |
| field_sfixed32_65 | [sfixed32](#sfixed32) | optional |  |
| field_sfixed64_66 | [sfixed64](#sfixed64) | optional |  |
| field_sint32_67 | [sint32](#sint32) | optional |  |
| field_sint64_68 | [sint64](#sint64) | optional |  |
| fieldgroup69 | [Proto2MessageLite.FieldGroup69](#protobuf-experimental-lite-Proto2MessageLite-FieldGroup69) | optional |  |
| field_required_double_71 | [double](#double) | required |  |
| field_required_float_72 | [float](#float) | required |  |
| field_required_int64_73 | [int64](#int64) | required |  |
| field_required_uint64_74 | [uint64](#uint64) | required |  |
| field_required_int32_75 | [int32](#int32) | required |  |
| field_required_fixed64_76 | [fixed64](#fixed64) | required |  |
| field_required_fixed32_77 | [fixed32](#fixed32) | required |  |
| field_required_bool_78 | [bool](#bool) | required |  |
| field_required_string_79 | [string](#string) | required |  |
| field_required_message_80 | [Proto2MessageLite.RequiredNestedMessage](#protobuf-experimental-lite-Proto2MessageLite-RequiredNestedMessage) | required |  |
| field_required_bytes_81 | [bytes](#bytes) | required |  |
| field_required_uint32_82 | [uint32](#uint32) | required |  |
| field_required_enum_83 | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | required |  |
| field_required_sfixed32_84 | [sfixed32](#sfixed32) | required |  |
| field_required_sfixed64_85 | [sfixed64](#sfixed64) | required |  |
| field_required_sint32_86 | [sint32](#sint32) | required |  |
| field_required_sint64_87 | [sint64](#sint64) | required |  |
| fieldrequiredgroup88 | [Proto2MessageLite.FieldRequiredGroup88](#protobuf-experimental-lite-Proto2MessageLite-FieldRequiredGroup88) | required |  |






<a name="protobuf-experimental-lite-Proto2MessageLite-FieldGroup49"></a>

### Proto2MessageLite.FieldGroup49



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_50 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLite-FieldGroup69"></a>

### Proto2MessageLite.FieldGroup69



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_70 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLite-FieldGroupList51"></a>

### Proto2MessageLite.FieldGroupList51



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_52 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLite-FieldRequiredGroup88"></a>

### Proto2MessageLite.FieldRequiredGroup88



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_89 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLite-RequiredNestedMessage"></a>

### Proto2MessageLite.RequiredNestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithExtensions"></a>

### Proto2MessageLiteWithExtensions







<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps"></a>

### Proto2MessageLiteWithMaps



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_map_bool_bool_1 | [Proto2MessageLiteWithMaps.FieldMapBoolBool1Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolBool1Entry) | repeated |  |
| field_map_bool_bytes_2 | [Proto2MessageLiteWithMaps.FieldMapBoolBytes2Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolBytes2Entry) | repeated |  |
| field_map_bool_double_3 | [Proto2MessageLiteWithMaps.FieldMapBoolDouble3Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolDouble3Entry) | repeated |  |
| field_map_bool_enum_4 | [Proto2MessageLiteWithMaps.FieldMapBoolEnum4Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolEnum4Entry) | repeated |  |
| field_map_bool_fixed32_5 | [Proto2MessageLiteWithMaps.FieldMapBoolFixed325Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFixed325Entry) | repeated |  |
| field_map_bool_fixed64_6 | [Proto2MessageLiteWithMaps.FieldMapBoolFixed646Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFixed646Entry) | repeated |  |
| field_map_bool_float_7 | [Proto2MessageLiteWithMaps.FieldMapBoolFloat7Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFloat7Entry) | repeated |  |
| field_map_bool_int32_8 | [Proto2MessageLiteWithMaps.FieldMapBoolInt328Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolInt328Entry) | repeated |  |
| field_map_bool_int64_9 | [Proto2MessageLiteWithMaps.FieldMapBoolInt649Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolInt649Entry) | repeated |  |
| field_map_bool_message_10 | [Proto2MessageLiteWithMaps.FieldMapBoolMessage10Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolMessage10Entry) | repeated |  |
| field_map_bool_sfixed32_11 | [Proto2MessageLiteWithMaps.FieldMapBoolSfixed3211Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSfixed3211Entry) | repeated |  |
| field_map_bool_sfixed64_12 | [Proto2MessageLiteWithMaps.FieldMapBoolSfixed6412Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSfixed6412Entry) | repeated |  |
| field_map_bool_sint32_13 | [Proto2MessageLiteWithMaps.FieldMapBoolSint3213Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSint3213Entry) | repeated |  |
| field_map_bool_sint64_14 | [Proto2MessageLiteWithMaps.FieldMapBoolSint6414Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSint6414Entry) | repeated |  |
| field_map_bool_string_15 | [Proto2MessageLiteWithMaps.FieldMapBoolString15Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolString15Entry) | repeated |  |
| field_map_bool_uint32_16 | [Proto2MessageLiteWithMaps.FieldMapBoolUint3216Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolUint3216Entry) | repeated |  |
| field_map_bool_uint64_17 | [Proto2MessageLiteWithMaps.FieldMapBoolUint6417Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolUint6417Entry) | repeated |  |
| field_map_fixed32_bool_18 | [Proto2MessageLiteWithMaps.FieldMapFixed32Bool18Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Bool18Entry) | repeated |  |
| field_map_fixed32_bytes_19 | [Proto2MessageLiteWithMaps.FieldMapFixed32Bytes19Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Bytes19Entry) | repeated |  |
| field_map_fixed32_double_20 | [Proto2MessageLiteWithMaps.FieldMapFixed32Double20Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Double20Entry) | repeated |  |
| field_map_fixed32_enum_21 | [Proto2MessageLiteWithMaps.FieldMapFixed32Enum21Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Enum21Entry) | repeated |  |
| field_map_fixed32_fixed32_22 | [Proto2MessageLiteWithMaps.FieldMapFixed32Fixed3222Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Fixed3222Entry) | repeated |  |
| field_map_fixed32_fixed64_23 | [Proto2MessageLiteWithMaps.FieldMapFixed32Fixed6423Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Fixed6423Entry) | repeated |  |
| field_map_fixed32_float_24 | [Proto2MessageLiteWithMaps.FieldMapFixed32Float24Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Float24Entry) | repeated |  |
| field_map_fixed32_int32_25 | [Proto2MessageLiteWithMaps.FieldMapFixed32Int3225Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Int3225Entry) | repeated |  |
| field_map_fixed32_int64_26 | [Proto2MessageLiteWithMaps.FieldMapFixed32Int6426Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Int6426Entry) | repeated |  |
| field_map_fixed32_message_27 | [Proto2MessageLiteWithMaps.FieldMapFixed32Message27Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Message27Entry) | repeated |  |
| field_map_fixed32_sfixed32_28 | [Proto2MessageLiteWithMaps.FieldMapFixed32Sfixed3228Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sfixed3228Entry) | repeated |  |
| field_map_fixed32_sfixed64_29 | [Proto2MessageLiteWithMaps.FieldMapFixed32Sfixed6429Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sfixed6429Entry) | repeated |  |
| field_map_fixed32_sint32_30 | [Proto2MessageLiteWithMaps.FieldMapFixed32Sint3230Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sint3230Entry) | repeated |  |
| field_map_fixed32_sint64_31 | [Proto2MessageLiteWithMaps.FieldMapFixed32Sint6431Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sint6431Entry) | repeated |  |
| field_map_fixed32_string_32 | [Proto2MessageLiteWithMaps.FieldMapFixed32String32Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32String32Entry) | repeated |  |
| field_map_fixed32_uint32_33 | [Proto2MessageLiteWithMaps.FieldMapFixed32Uint3233Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Uint3233Entry) | repeated |  |
| field_map_fixed32_uint64_34 | [Proto2MessageLiteWithMaps.FieldMapFixed32Uint6434Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Uint6434Entry) | repeated |  |
| field_map_fixed64_bool_35 | [Proto2MessageLiteWithMaps.FieldMapFixed64Bool35Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Bool35Entry) | repeated |  |
| field_map_fixed64_bytes_36 | [Proto2MessageLiteWithMaps.FieldMapFixed64Bytes36Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Bytes36Entry) | repeated |  |
| field_map_fixed64_double_37 | [Proto2MessageLiteWithMaps.FieldMapFixed64Double37Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Double37Entry) | repeated |  |
| field_map_fixed64_enum_38 | [Proto2MessageLiteWithMaps.FieldMapFixed64Enum38Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Enum38Entry) | repeated |  |
| field_map_fixed64_fixed32_39 | [Proto2MessageLiteWithMaps.FieldMapFixed64Fixed3239Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Fixed3239Entry) | repeated |  |
| field_map_fixed64_fixed64_40 | [Proto2MessageLiteWithMaps.FieldMapFixed64Fixed6440Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Fixed6440Entry) | repeated |  |
| field_map_fixed64_float_41 | [Proto2MessageLiteWithMaps.FieldMapFixed64Float41Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Float41Entry) | repeated |  |
| field_map_fixed64_int32_42 | [Proto2MessageLiteWithMaps.FieldMapFixed64Int3242Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Int3242Entry) | repeated |  |
| field_map_fixed64_int64_43 | [Proto2MessageLiteWithMaps.FieldMapFixed64Int6443Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Int6443Entry) | repeated |  |
| field_map_fixed64_message_44 | [Proto2MessageLiteWithMaps.FieldMapFixed64Message44Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Message44Entry) | repeated |  |
| field_map_fixed64_sfixed32_45 | [Proto2MessageLiteWithMaps.FieldMapFixed64Sfixed3245Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sfixed3245Entry) | repeated |  |
| field_map_fixed64_sfixed64_46 | [Proto2MessageLiteWithMaps.FieldMapFixed64Sfixed6446Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sfixed6446Entry) | repeated |  |
| field_map_fixed64_sint32_47 | [Proto2MessageLiteWithMaps.FieldMapFixed64Sint3247Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sint3247Entry) | repeated |  |
| field_map_fixed64_sint64_48 | [Proto2MessageLiteWithMaps.FieldMapFixed64Sint6448Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sint6448Entry) | repeated |  |
| field_map_fixed64_string_49 | [Proto2MessageLiteWithMaps.FieldMapFixed64String49Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64String49Entry) | repeated |  |
| field_map_fixed64_uint32_50 | [Proto2MessageLiteWithMaps.FieldMapFixed64Uint3250Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Uint3250Entry) | repeated |  |
| field_map_fixed64_uint64_51 | [Proto2MessageLiteWithMaps.FieldMapFixed64Uint6451Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Uint6451Entry) | repeated |  |
| field_map_int32_bool_52 | [Proto2MessageLiteWithMaps.FieldMapInt32Bool52Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Bool52Entry) | repeated |  |
| field_map_int32_bytes_53 | [Proto2MessageLiteWithMaps.FieldMapInt32Bytes53Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Bytes53Entry) | repeated |  |
| field_map_int32_double_54 | [Proto2MessageLiteWithMaps.FieldMapInt32Double54Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Double54Entry) | repeated |  |
| field_map_int32_enum_55 | [Proto2MessageLiteWithMaps.FieldMapInt32Enum55Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Enum55Entry) | repeated |  |
| field_map_int32_fixed32_56 | [Proto2MessageLiteWithMaps.FieldMapInt32Fixed3256Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Fixed3256Entry) | repeated |  |
| field_map_int32_fixed64_57 | [Proto2MessageLiteWithMaps.FieldMapInt32Fixed6457Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Fixed6457Entry) | repeated |  |
| field_map_int32_float_58 | [Proto2MessageLiteWithMaps.FieldMapInt32Float58Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Float58Entry) | repeated |  |
| field_map_int32_int32_59 | [Proto2MessageLiteWithMaps.FieldMapInt32Int3259Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Int3259Entry) | repeated |  |
| field_map_int32_int64_60 | [Proto2MessageLiteWithMaps.FieldMapInt32Int6460Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Int6460Entry) | repeated |  |
| field_map_int32_message_61 | [Proto2MessageLiteWithMaps.FieldMapInt32Message61Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Message61Entry) | repeated |  |
| field_map_int32_sfixed32_62 | [Proto2MessageLiteWithMaps.FieldMapInt32Sfixed3262Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sfixed3262Entry) | repeated |  |
| field_map_int32_sfixed64_63 | [Proto2MessageLiteWithMaps.FieldMapInt32Sfixed6463Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sfixed6463Entry) | repeated |  |
| field_map_int32_sint32_64 | [Proto2MessageLiteWithMaps.FieldMapInt32Sint3264Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sint3264Entry) | repeated |  |
| field_map_int32_sint64_65 | [Proto2MessageLiteWithMaps.FieldMapInt32Sint6465Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sint6465Entry) | repeated |  |
| field_map_int32_string_66 | [Proto2MessageLiteWithMaps.FieldMapInt32String66Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32String66Entry) | repeated |  |
| field_map_int32_uint32_67 | [Proto2MessageLiteWithMaps.FieldMapInt32Uint3267Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Uint3267Entry) | repeated |  |
| field_map_int32_uint64_68 | [Proto2MessageLiteWithMaps.FieldMapInt32Uint6468Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Uint6468Entry) | repeated |  |
| field_map_int64_bool_69 | [Proto2MessageLiteWithMaps.FieldMapInt64Bool69Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Bool69Entry) | repeated |  |
| field_map_int64_bytes_70 | [Proto2MessageLiteWithMaps.FieldMapInt64Bytes70Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Bytes70Entry) | repeated |  |
| field_map_int64_double_71 | [Proto2MessageLiteWithMaps.FieldMapInt64Double71Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Double71Entry) | repeated |  |
| field_map_int64_enum_72 | [Proto2MessageLiteWithMaps.FieldMapInt64Enum72Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Enum72Entry) | repeated |  |
| field_map_int64_fixed32_73 | [Proto2MessageLiteWithMaps.FieldMapInt64Fixed3273Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Fixed3273Entry) | repeated |  |
| field_map_int64_fixed64_74 | [Proto2MessageLiteWithMaps.FieldMapInt64Fixed6474Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Fixed6474Entry) | repeated |  |
| field_map_int64_float_75 | [Proto2MessageLiteWithMaps.FieldMapInt64Float75Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Float75Entry) | repeated |  |
| field_map_int64_int32_76 | [Proto2MessageLiteWithMaps.FieldMapInt64Int3276Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Int3276Entry) | repeated |  |
| field_map_int64_int64_77 | [Proto2MessageLiteWithMaps.FieldMapInt64Int6477Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Int6477Entry) | repeated |  |
| field_map_int64_message_78 | [Proto2MessageLiteWithMaps.FieldMapInt64Message78Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Message78Entry) | repeated |  |
| field_map_int64_sfixed32_79 | [Proto2MessageLiteWithMaps.FieldMapInt64Sfixed3279Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sfixed3279Entry) | repeated |  |
| field_map_int64_sfixed64_80 | [Proto2MessageLiteWithMaps.FieldMapInt64Sfixed6480Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sfixed6480Entry) | repeated |  |
| field_map_int64_sint32_81 | [Proto2MessageLiteWithMaps.FieldMapInt64Sint3281Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sint3281Entry) | repeated |  |
| field_map_int64_sint64_82 | [Proto2MessageLiteWithMaps.FieldMapInt64Sint6482Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sint6482Entry) | repeated |  |
| field_map_int64_string_83 | [Proto2MessageLiteWithMaps.FieldMapInt64String83Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64String83Entry) | repeated |  |
| field_map_int64_uint32_84 | [Proto2MessageLiteWithMaps.FieldMapInt64Uint3284Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Uint3284Entry) | repeated |  |
| field_map_int64_uint64_85 | [Proto2MessageLiteWithMaps.FieldMapInt64Uint6485Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Uint6485Entry) | repeated |  |
| field_map_sfixed32_bool_86 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Bool86Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Bool86Entry) | repeated |  |
| field_map_sfixed32_bytes_87 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Bytes87Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Bytes87Entry) | repeated |  |
| field_map_sfixed32_double_88 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Double88Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Double88Entry) | repeated |  |
| field_map_sfixed32_enum_89 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Enum89Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Enum89Entry) | repeated |  |
| field_map_sfixed32_fixed32_90 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Fixed3290Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Fixed3290Entry) | repeated |  |
| field_map_sfixed32_fixed64_91 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Fixed6491Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Fixed6491Entry) | repeated |  |
| field_map_sfixed32_float_92 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Float92Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Float92Entry) | repeated |  |
| field_map_sfixed32_int32_93 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Int3293Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Int3293Entry) | repeated |  |
| field_map_sfixed32_int64_94 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Int6494Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Int6494Entry) | repeated |  |
| field_map_sfixed32_message_95 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Message95Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Message95Entry) | repeated |  |
| field_map_sfixed32_sfixed32_96 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Sfixed3296Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sfixed3296Entry) | repeated |  |
| field_map_sfixed32_sfixed64_97 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Sfixed6497Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sfixed6497Entry) | repeated |  |
| field_map_sfixed32_sint32_98 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Sint3298Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sint3298Entry) | repeated |  |
| field_map_sfixed32_sint64_99 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Sint6499Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sint6499Entry) | repeated |  |
| field_map_sfixed32_string_100 | [Proto2MessageLiteWithMaps.FieldMapSfixed32String100Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32String100Entry) | repeated |  |
| field_map_sfixed32_uint32_101 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Uint32101Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Uint32101Entry) | repeated |  |
| field_map_sfixed32_uint64_102 | [Proto2MessageLiteWithMaps.FieldMapSfixed32Uint64102Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Uint64102Entry) | repeated |  |
| field_map_sfixed64_bool_103 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Bool103Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Bool103Entry) | repeated |  |
| field_map_sfixed64_bytes_104 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Bytes104Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Bytes104Entry) | repeated |  |
| field_map_sfixed64_double_105 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Double105Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Double105Entry) | repeated |  |
| field_map_sfixed64_enum_106 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Enum106Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Enum106Entry) | repeated |  |
| field_map_sfixed64_fixed32_107 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Fixed32107Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Fixed32107Entry) | repeated |  |
| field_map_sfixed64_fixed64_108 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Fixed64108Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Fixed64108Entry) | repeated |  |
| field_map_sfixed64_float_109 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Float109Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Float109Entry) | repeated |  |
| field_map_sfixed64_int32_110 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Int32110Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Int32110Entry) | repeated |  |
| field_map_sfixed64_int64_111 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Int64111Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Int64111Entry) | repeated |  |
| field_map_sfixed64_message_112 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Message112Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Message112Entry) | repeated |  |
| field_map_sfixed64_sfixed32_113 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Sfixed32113Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sfixed32113Entry) | repeated |  |
| field_map_sfixed64_sfixed64_114 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Sfixed64114Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sfixed64114Entry) | repeated |  |
| field_map_sfixed64_sint32_115 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Sint32115Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sint32115Entry) | repeated |  |
| field_map_sfixed64_sint64_116 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Sint64116Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sint64116Entry) | repeated |  |
| field_map_sfixed64_string_117 | [Proto2MessageLiteWithMaps.FieldMapSfixed64String117Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64String117Entry) | repeated |  |
| field_map_sfixed64_uint32_118 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Uint32118Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Uint32118Entry) | repeated |  |
| field_map_sfixed64_uint64_119 | [Proto2MessageLiteWithMaps.FieldMapSfixed64Uint64119Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Uint64119Entry) | repeated |  |
| field_map_sint32_bool_120 | [Proto2MessageLiteWithMaps.FieldMapSint32Bool120Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Bool120Entry) | repeated |  |
| field_map_sint32_bytes_121 | [Proto2MessageLiteWithMaps.FieldMapSint32Bytes121Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Bytes121Entry) | repeated |  |
| field_map_sint32_double_122 | [Proto2MessageLiteWithMaps.FieldMapSint32Double122Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Double122Entry) | repeated |  |
| field_map_sint32_enum_123 | [Proto2MessageLiteWithMaps.FieldMapSint32Enum123Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Enum123Entry) | repeated |  |
| field_map_sint32_fixed32_124 | [Proto2MessageLiteWithMaps.FieldMapSint32Fixed32124Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Fixed32124Entry) | repeated |  |
| field_map_sint32_fixed64_125 | [Proto2MessageLiteWithMaps.FieldMapSint32Fixed64125Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Fixed64125Entry) | repeated |  |
| field_map_sint32_float_126 | [Proto2MessageLiteWithMaps.FieldMapSint32Float126Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Float126Entry) | repeated |  |
| field_map_sint32_int32_127 | [Proto2MessageLiteWithMaps.FieldMapSint32Int32127Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Int32127Entry) | repeated |  |
| field_map_sint32_int64_128 | [Proto2MessageLiteWithMaps.FieldMapSint32Int64128Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Int64128Entry) | repeated |  |
| field_map_sint32_message_129 | [Proto2MessageLiteWithMaps.FieldMapSint32Message129Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Message129Entry) | repeated |  |
| field_map_sint32_sfixed32_130 | [Proto2MessageLiteWithMaps.FieldMapSint32Sfixed32130Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sfixed32130Entry) | repeated |  |
| field_map_sint32_sfixed64_131 | [Proto2MessageLiteWithMaps.FieldMapSint32Sfixed64131Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sfixed64131Entry) | repeated |  |
| field_map_sint32_sint32_132 | [Proto2MessageLiteWithMaps.FieldMapSint32Sint32132Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sint32132Entry) | repeated |  |
| field_map_sint32_sint64_133 | [Proto2MessageLiteWithMaps.FieldMapSint32Sint64133Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sint64133Entry) | repeated |  |
| field_map_sint32_string_134 | [Proto2MessageLiteWithMaps.FieldMapSint32String134Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32String134Entry) | repeated |  |
| field_map_sint32_uint32_135 | [Proto2MessageLiteWithMaps.FieldMapSint32Uint32135Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Uint32135Entry) | repeated |  |
| field_map_sint32_uint64_136 | [Proto2MessageLiteWithMaps.FieldMapSint32Uint64136Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Uint64136Entry) | repeated |  |
| field_map_sint64_bool_137 | [Proto2MessageLiteWithMaps.FieldMapSint64Bool137Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Bool137Entry) | repeated |  |
| field_map_sint64_bytes_138 | [Proto2MessageLiteWithMaps.FieldMapSint64Bytes138Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Bytes138Entry) | repeated |  |
| field_map_sint64_double_139 | [Proto2MessageLiteWithMaps.FieldMapSint64Double139Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Double139Entry) | repeated |  |
| field_map_sint64_enum_140 | [Proto2MessageLiteWithMaps.FieldMapSint64Enum140Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Enum140Entry) | repeated |  |
| field_map_sint64_fixed32_141 | [Proto2MessageLiteWithMaps.FieldMapSint64Fixed32141Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Fixed32141Entry) | repeated |  |
| field_map_sint64_fixed64_142 | [Proto2MessageLiteWithMaps.FieldMapSint64Fixed64142Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Fixed64142Entry) | repeated |  |
| field_map_sint64_float_143 | [Proto2MessageLiteWithMaps.FieldMapSint64Float143Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Float143Entry) | repeated |  |
| field_map_sint64_int32_144 | [Proto2MessageLiteWithMaps.FieldMapSint64Int32144Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Int32144Entry) | repeated |  |
| field_map_sint64_int64_145 | [Proto2MessageLiteWithMaps.FieldMapSint64Int64145Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Int64145Entry) | repeated |  |
| field_map_sint64_message_146 | [Proto2MessageLiteWithMaps.FieldMapSint64Message146Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Message146Entry) | repeated |  |
| field_map_sint64_sfixed32_147 | [Proto2MessageLiteWithMaps.FieldMapSint64Sfixed32147Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sfixed32147Entry) | repeated |  |
| field_map_sint64_sfixed64_148 | [Proto2MessageLiteWithMaps.FieldMapSint64Sfixed64148Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sfixed64148Entry) | repeated |  |
| field_map_sint64_sint32_149 | [Proto2MessageLiteWithMaps.FieldMapSint64Sint32149Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sint32149Entry) | repeated |  |
| field_map_sint64_sint64_150 | [Proto2MessageLiteWithMaps.FieldMapSint64Sint64150Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sint64150Entry) | repeated |  |
| field_map_sint64_string_151 | [Proto2MessageLiteWithMaps.FieldMapSint64String151Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64String151Entry) | repeated |  |
| field_map_sint64_uint32_152 | [Proto2MessageLiteWithMaps.FieldMapSint64Uint32152Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Uint32152Entry) | repeated |  |
| field_map_sint64_uint64_153 | [Proto2MessageLiteWithMaps.FieldMapSint64Uint64153Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Uint64153Entry) | repeated |  |
| field_map_string_bool_154 | [Proto2MessageLiteWithMaps.FieldMapStringBool154Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringBool154Entry) | repeated |  |
| field_map_string_bytes_155 | [Proto2MessageLiteWithMaps.FieldMapStringBytes155Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringBytes155Entry) | repeated |  |
| field_map_string_double_156 | [Proto2MessageLiteWithMaps.FieldMapStringDouble156Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringDouble156Entry) | repeated |  |
| field_map_string_enum_157 | [Proto2MessageLiteWithMaps.FieldMapStringEnum157Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringEnum157Entry) | repeated |  |
| field_map_string_fixed32_158 | [Proto2MessageLiteWithMaps.FieldMapStringFixed32158Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFixed32158Entry) | repeated |  |
| field_map_string_fixed64_159 | [Proto2MessageLiteWithMaps.FieldMapStringFixed64159Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFixed64159Entry) | repeated |  |
| field_map_string_float_160 | [Proto2MessageLiteWithMaps.FieldMapStringFloat160Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFloat160Entry) | repeated |  |
| field_map_string_int32_161 | [Proto2MessageLiteWithMaps.FieldMapStringInt32161Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringInt32161Entry) | repeated |  |
| field_map_string_int64_162 | [Proto2MessageLiteWithMaps.FieldMapStringInt64162Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringInt64162Entry) | repeated |  |
| field_map_string_message_163 | [Proto2MessageLiteWithMaps.FieldMapStringMessage163Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringMessage163Entry) | repeated |  |
| field_map_string_sfixed32_164 | [Proto2MessageLiteWithMaps.FieldMapStringSfixed32164Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSfixed32164Entry) | repeated |  |
| field_map_string_sfixed64_165 | [Proto2MessageLiteWithMaps.FieldMapStringSfixed64165Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSfixed64165Entry) | repeated |  |
| field_map_string_sint32_166 | [Proto2MessageLiteWithMaps.FieldMapStringSint32166Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSint32166Entry) | repeated |  |
| field_map_string_sint64_167 | [Proto2MessageLiteWithMaps.FieldMapStringSint64167Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSint64167Entry) | repeated |  |
| field_map_string_string_168 | [Proto2MessageLiteWithMaps.FieldMapStringString168Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringString168Entry) | repeated |  |
| field_map_string_uint32_169 | [Proto2MessageLiteWithMaps.FieldMapStringUint32169Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringUint32169Entry) | repeated |  |
| field_map_string_uint64_170 | [Proto2MessageLiteWithMaps.FieldMapStringUint64170Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringUint64170Entry) | repeated |  |
| field_map_uint32_bool_171 | [Proto2MessageLiteWithMaps.FieldMapUint32Bool171Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Bool171Entry) | repeated |  |
| field_map_uint32_bytes_172 | [Proto2MessageLiteWithMaps.FieldMapUint32Bytes172Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Bytes172Entry) | repeated |  |
| field_map_uint32_double_173 | [Proto2MessageLiteWithMaps.FieldMapUint32Double173Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Double173Entry) | repeated |  |
| field_map_uint32_enum_174 | [Proto2MessageLiteWithMaps.FieldMapUint32Enum174Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Enum174Entry) | repeated |  |
| field_map_uint32_fixed32_175 | [Proto2MessageLiteWithMaps.FieldMapUint32Fixed32175Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Fixed32175Entry) | repeated |  |
| field_map_uint32_fixed64_176 | [Proto2MessageLiteWithMaps.FieldMapUint32Fixed64176Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Fixed64176Entry) | repeated |  |
| field_map_uint32_float_177 | [Proto2MessageLiteWithMaps.FieldMapUint32Float177Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Float177Entry) | repeated |  |
| field_map_uint32_int32_178 | [Proto2MessageLiteWithMaps.FieldMapUint32Int32178Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Int32178Entry) | repeated |  |
| field_map_uint32_int64_179 | [Proto2MessageLiteWithMaps.FieldMapUint32Int64179Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Int64179Entry) | repeated |  |
| field_map_uint32_message_180 | [Proto2MessageLiteWithMaps.FieldMapUint32Message180Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Message180Entry) | repeated |  |
| field_map_uint32_sfixed32_181 | [Proto2MessageLiteWithMaps.FieldMapUint32Sfixed32181Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sfixed32181Entry) | repeated |  |
| field_map_uint32_sfixed64_182 | [Proto2MessageLiteWithMaps.FieldMapUint32Sfixed64182Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sfixed64182Entry) | repeated |  |
| field_map_uint32_sint32_183 | [Proto2MessageLiteWithMaps.FieldMapUint32Sint32183Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sint32183Entry) | repeated |  |
| field_map_uint32_sint64_184 | [Proto2MessageLiteWithMaps.FieldMapUint32Sint64184Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sint64184Entry) | repeated |  |
| field_map_uint32_string_185 | [Proto2MessageLiteWithMaps.FieldMapUint32String185Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32String185Entry) | repeated |  |
| field_map_uint32_uint32_186 | [Proto2MessageLiteWithMaps.FieldMapUint32Uint32186Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Uint32186Entry) | repeated |  |
| field_map_uint32_uint64_187 | [Proto2MessageLiteWithMaps.FieldMapUint32Uint64187Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Uint64187Entry) | repeated |  |
| field_map_uint64_bool_188 | [Proto2MessageLiteWithMaps.FieldMapUint64Bool188Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Bool188Entry) | repeated |  |
| field_map_uint64_bytes_189 | [Proto2MessageLiteWithMaps.FieldMapUint64Bytes189Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Bytes189Entry) | repeated |  |
| field_map_uint64_double_190 | [Proto2MessageLiteWithMaps.FieldMapUint64Double190Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Double190Entry) | repeated |  |
| field_map_uint64_enum_191 | [Proto2MessageLiteWithMaps.FieldMapUint64Enum191Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Enum191Entry) | repeated |  |
| field_map_uint64_fixed32_192 | [Proto2MessageLiteWithMaps.FieldMapUint64Fixed32192Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Fixed32192Entry) | repeated |  |
| field_map_uint64_fixed64_193 | [Proto2MessageLiteWithMaps.FieldMapUint64Fixed64193Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Fixed64193Entry) | repeated |  |
| field_map_uint64_float_194 | [Proto2MessageLiteWithMaps.FieldMapUint64Float194Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Float194Entry) | repeated |  |
| field_map_uint64_int32_195 | [Proto2MessageLiteWithMaps.FieldMapUint64Int32195Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Int32195Entry) | repeated |  |
| field_map_uint64_int64_196 | [Proto2MessageLiteWithMaps.FieldMapUint64Int64196Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Int64196Entry) | repeated |  |
| field_map_uint64_message_197 | [Proto2MessageLiteWithMaps.FieldMapUint64Message197Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Message197Entry) | repeated |  |
| field_map_uint64_sfixed32_198 | [Proto2MessageLiteWithMaps.FieldMapUint64Sfixed32198Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sfixed32198Entry) | repeated |  |
| field_map_uint64_sfixed64_199 | [Proto2MessageLiteWithMaps.FieldMapUint64Sfixed64199Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sfixed64199Entry) | repeated |  |
| field_map_uint64_sint32_200 | [Proto2MessageLiteWithMaps.FieldMapUint64Sint32200Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sint32200Entry) | repeated |  |
| field_map_uint64_sint64_201 | [Proto2MessageLiteWithMaps.FieldMapUint64Sint64201Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sint64201Entry) | repeated |  |
| field_map_uint64_string_202 | [Proto2MessageLiteWithMaps.FieldMapUint64String202Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64String202Entry) | repeated |  |
| field_map_uint64_uint32_203 | [Proto2MessageLiteWithMaps.FieldMapUint64Uint32203Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Uint32203Entry) | repeated |  |
| field_map_uint64_uint64_204 | [Proto2MessageLiteWithMaps.FieldMapUint64Uint64204Entry](#protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Uint64204Entry) | repeated |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolBool1Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolBool1Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolBytes2Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolBytes2Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolDouble3Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolDouble3Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolEnum4Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolEnum4Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFixed325Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolFixed325Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFixed646Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolFixed646Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolFloat7Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolFloat7Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolInt328Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolInt328Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolInt649Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolInt649Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolMessage10Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolMessage10Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSfixed3211Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolSfixed3211Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSfixed6412Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolSfixed6412Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSint3213Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolSint3213Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolSint6414Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolSint6414Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolString15Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolString15Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolUint3216Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolUint3216Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapBoolUint6417Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapBoolUint6417Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Bool18Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Bool18Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Bytes19Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Bytes19Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Double20Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Double20Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Enum21Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Enum21Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Fixed3222Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Fixed3222Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Fixed6423Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Fixed6423Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Float24Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Float24Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Int3225Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Int3225Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Int6426Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Int6426Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Message27Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Message27Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sfixed3228Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Sfixed3228Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sfixed6429Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Sfixed6429Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sint3230Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Sint3230Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Sint6431Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Sint6431Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32String32Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32String32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Uint3233Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Uint3233Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed32Uint6434Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed32Uint6434Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Bool35Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Bool35Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Bytes36Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Bytes36Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Double37Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Double37Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Enum38Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Enum38Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Fixed3239Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Fixed3239Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Fixed6440Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Fixed6440Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Float41Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Float41Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Int3242Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Int3242Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Int6443Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Int6443Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Message44Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Message44Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sfixed3245Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Sfixed3245Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sfixed6446Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Sfixed6446Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sint3247Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Sint3247Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Sint6448Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Sint6448Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64String49Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64String49Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Uint3250Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Uint3250Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapFixed64Uint6451Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapFixed64Uint6451Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Bool52Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Bool52Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Bytes53Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Bytes53Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Double54Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Double54Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Enum55Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Enum55Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Fixed3256Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Fixed3256Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Fixed6457Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Fixed6457Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Float58Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Float58Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Int3259Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Int3259Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Int6460Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Int6460Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Message61Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Message61Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sfixed3262Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Sfixed3262Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sfixed6463Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Sfixed6463Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sint3264Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Sint3264Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Sint6465Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Sint6465Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32String66Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32String66Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Uint3267Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Uint3267Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt32Uint6468Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt32Uint6468Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Bool69Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Bool69Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Bytes70Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Bytes70Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Double71Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Double71Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Enum72Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Enum72Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Fixed3273Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Fixed3273Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Fixed6474Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Fixed6474Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Float75Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Float75Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Int3276Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Int3276Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Int6477Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Int6477Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Message78Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Message78Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sfixed3279Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Sfixed3279Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sfixed6480Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Sfixed6480Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sint3281Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Sint3281Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Sint6482Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Sint6482Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64String83Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64String83Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Uint3284Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Uint3284Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapInt64Uint6485Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapInt64Uint6485Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Bool86Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Bool86Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Bytes87Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Bytes87Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Double88Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Double88Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Enum89Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Enum89Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Fixed3290Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Fixed3290Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Fixed6491Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Fixed6491Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Float92Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Float92Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Int3293Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Int3293Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Int6494Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Int6494Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Message95Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Message95Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sfixed3296Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Sfixed3296Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sfixed6497Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Sfixed6497Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sint3298Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Sint3298Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Sint6499Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Sint6499Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32String100Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32String100Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Uint32101Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Uint32101Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed32Uint64102Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed32Uint64102Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Bool103Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Bool103Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Bytes104Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Bytes104Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Double105Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Double105Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Enum106Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Enum106Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Fixed32107Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Fixed32107Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Fixed64108Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Fixed64108Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Float109Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Float109Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Int32110Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Int32110Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Int64111Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Int64111Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Message112Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Message112Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sfixed32113Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Sfixed32113Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sfixed64114Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Sfixed64114Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sint32115Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Sint32115Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Sint64116Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Sint64116Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64String117Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64String117Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Uint32118Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Uint32118Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSfixed64Uint64119Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSfixed64Uint64119Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Bool120Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Bool120Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Bytes121Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Bytes121Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Double122Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Double122Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Enum123Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Enum123Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Fixed32124Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Fixed32124Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Fixed64125Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Fixed64125Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Float126Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Float126Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Int32127Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Int32127Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Int64128Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Int64128Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Message129Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Message129Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sfixed32130Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Sfixed32130Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sfixed64131Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Sfixed64131Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sint32132Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Sint32132Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Sint64133Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Sint64133Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32String134Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32String134Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Uint32135Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Uint32135Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint32Uint64136Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint32Uint64136Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Bool137Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Bool137Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Bytes138Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Bytes138Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Double139Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Double139Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Enum140Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Enum140Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Fixed32141Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Fixed32141Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Fixed64142Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Fixed64142Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Float143Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Float143Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Int32144Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Int32144Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Int64145Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Int64145Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Message146Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Message146Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sfixed32147Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Sfixed32147Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sfixed64148Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Sfixed64148Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sint32149Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Sint32149Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Sint64150Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Sint64150Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64String151Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64String151Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Uint32152Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Uint32152Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapSint64Uint64153Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapSint64Uint64153Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringBool154Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringBool154Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringBytes155Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringBytes155Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringDouble156Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringDouble156Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringEnum157Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringEnum157Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFixed32158Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringFixed32158Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFixed64159Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringFixed64159Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringFloat160Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringFloat160Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringInt32161Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringInt32161Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringInt64162Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringInt64162Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringMessage163Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringMessage163Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSfixed32164Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringSfixed32164Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSfixed64165Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringSfixed64165Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSint32166Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringSint32166Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringSint64167Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringSint64167Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringString168Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringString168Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringUint32169Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringUint32169Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapStringUint64170Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapStringUint64170Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Bool171Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Bool171Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Bytes172Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Bytes172Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Double173Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Double173Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Enum174Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Enum174Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Fixed32175Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Fixed32175Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Fixed64176Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Fixed64176Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Float177Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Float177Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Int32178Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Int32178Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Int64179Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Int64179Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Message180Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Message180Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sfixed32181Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Sfixed32181Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sfixed64182Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Sfixed64182Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sint32183Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Sint32183Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Sint64184Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Sint64184Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32String185Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32String185Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Uint32186Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Uint32186Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint32Uint64187Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint32Uint64187Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Bool188Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Bool188Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Bytes189Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Bytes189Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Double190Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Double190Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Enum191Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Enum191Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [Proto2MessageLite.TestEnum](#protobuf-experimental-lite-Proto2MessageLite-TestEnum) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Fixed32192Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Fixed32192Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Fixed64193Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Fixed64193Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Float194Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Float194Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Int32195Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Int32195Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Int64196Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Int64196Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Message197Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Message197Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [Proto2MessageLite](#protobuf-experimental-lite-Proto2MessageLite) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sfixed32198Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Sfixed32198Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sfixed64199Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Sfixed64199Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sint32200Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Sint32200Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Sint64201Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Sint64201Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64String202Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64String202Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Uint32203Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Uint32203Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-lite-Proto2MessageLiteWithMaps-FieldMapUint64Uint64204Entry"></a>

### Proto2MessageLiteWithMaps.FieldMapUint64Uint64204Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [uint64](#uint64) | optional |  |





 


<a name="protobuf-experimental-lite-Proto2MessageLite-TestEnum"></a>

### Proto2MessageLite.TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |
| TWO | 2 |  |


 


<a name="java_core_src_test_proto_com_google_protobuf_proto2_message_lite-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| field_bool_8 | bool | Proto2MessageLiteWithExtensions | 8 |  |
| field_bool_list_25 | bool | Proto2MessageLiteWithExtensions | 25 |  |
| field_bool_list_packed_42 | bool | Proto2MessageLiteWithExtensions | 42 |  |
| field_bytes_11 | bytes | Proto2MessageLiteWithExtensions | 11 |  |
| field_bytes_list_28 | bytes | Proto2MessageLiteWithExtensions | 28 |  |
| field_double_1 | double | Proto2MessageLiteWithExtensions | 1 |  |
| field_double_list_18 | double | Proto2MessageLiteWithExtensions | 18 |  |
| field_double_list_packed_35 | double | Proto2MessageLiteWithExtensions | 35 |  |
| field_enum_13 | Proto2MessageLite.TestEnum | Proto2MessageLiteWithExtensions | 13 |  |
| field_enum_list_30 | Proto2MessageLite.TestEnum | Proto2MessageLiteWithExtensions | 30 |  |
| field_enum_list_packed_44 | Proto2MessageLite.TestEnum | Proto2MessageLiteWithExtensions | 44 |  |
| field_fixed32_7 | fixed32 | Proto2MessageLiteWithExtensions | 7 |  |
| field_fixed32_list_24 | fixed32 | Proto2MessageLiteWithExtensions | 24 |  |
| field_fixed32_list_packed_41 | fixed32 | Proto2MessageLiteWithExtensions | 41 |  |
| field_fixed64_6 | fixed64 | Proto2MessageLiteWithExtensions | 6 |  |
| field_fixed64_list_23 | fixed64 | Proto2MessageLiteWithExtensions | 23 |  |
| field_fixed64_list_packed_40 | fixed64 | Proto2MessageLiteWithExtensions | 40 |  |
| field_float_2 | float | Proto2MessageLiteWithExtensions | 2 |  |
| field_float_list_19 | float | Proto2MessageLiteWithExtensions | 19 |  |
| field_float_list_packed_36 | float | Proto2MessageLiteWithExtensions | 36 |  |
| field_int32_5 | int32 | Proto2MessageLiteWithExtensions | 5 |  |
| field_int32_list_22 | int32 | Proto2MessageLiteWithExtensions | 22 |  |
| field_int32_list_packed_39 | int32 | Proto2MessageLiteWithExtensions | 39 |  |
| field_int64_3 | int64 | Proto2MessageLiteWithExtensions | 3 |  |
| field_int64_list_20 | int64 | Proto2MessageLiteWithExtensions | 20 |  |
| field_int64_list_packed_37 | int64 | Proto2MessageLiteWithExtensions | 37 |  |
| field_message_10 | Proto2MessageLite | Proto2MessageLiteWithExtensions | 10 |  |
| field_message_list_27 | Proto2MessageLite | Proto2MessageLiteWithExtensions | 27 |  |
| field_sfixed32_14 | sfixed32 | Proto2MessageLiteWithExtensions | 14 |  |
| field_sfixed32_list_31 | sfixed32 | Proto2MessageLiteWithExtensions | 31 |  |
| field_sfixed32_list_packed_45 | sfixed32 | Proto2MessageLiteWithExtensions | 45 |  |
| field_sfixed64_15 | sfixed64 | Proto2MessageLiteWithExtensions | 15 |  |
| field_sfixed64_list_32 | sfixed64 | Proto2MessageLiteWithExtensions | 32 |  |
| field_sfixed64_list_packed_46 | sfixed64 | Proto2MessageLiteWithExtensions | 46 |  |
| field_sint32_16 | sint32 | Proto2MessageLiteWithExtensions | 16 |  |
| field_sint32_list_33 | sint32 | Proto2MessageLiteWithExtensions | 33 |  |
| field_sint32_list_packed_47 | sint32 | Proto2MessageLiteWithExtensions | 47 |  |
| field_sint64_17 | sint64 | Proto2MessageLiteWithExtensions | 17 |  |
| field_sint64_list_34 | sint64 | Proto2MessageLiteWithExtensions | 34 |  |
| field_sint64_list_packed_48 | sint64 | Proto2MessageLiteWithExtensions | 48 |  |
| field_string_9 | string | Proto2MessageLiteWithExtensions | 9 |  |
| field_string_list_26 | string | Proto2MessageLiteWithExtensions | 26 |  |
| field_uint32_12 | uint32 | Proto2MessageLiteWithExtensions | 12 |  |
| field_uint32_list_29 | uint32 | Proto2MessageLiteWithExtensions | 29 |  |
| field_uint32_list_packed_43 | uint32 | Proto2MessageLiteWithExtensions | 43 |  |
| field_uint64_4 | uint64 | Proto2MessageLiteWithExtensions | 4 |  |
| field_uint64_list_21 | uint64 | Proto2MessageLiteWithExtensions | 21 |  |
| field_uint64_list_packed_38 | uint64 | Proto2MessageLiteWithExtensions | 38 |  |
| fieldgroup49 | FieldGroup49 | Proto2MessageLiteWithExtensions | 49 |  |
| fieldgrouplist51 | FieldGroupList51 | Proto2MessageLiteWithExtensions | 51 |  |

 

 



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

