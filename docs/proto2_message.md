# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/core/src/test/proto/com/google/protobuf/proto2_message.proto](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto)
    - [FieldGroup49](#protobuf-experimental-FieldGroup49)
    - [FieldGroupList51](#protobuf-experimental-FieldGroupList51)
    - [Proto2Empty](#protobuf-experimental-Proto2Empty)
    - [Proto2Message](#protobuf-experimental-Proto2Message)
    - [Proto2Message.FieldGroup49](#protobuf-experimental-Proto2Message-FieldGroup49)
    - [Proto2Message.FieldGroup69](#protobuf-experimental-Proto2Message-FieldGroup69)
    - [Proto2Message.FieldGroupList51](#protobuf-experimental-Proto2Message-FieldGroupList51)
    - [Proto2Message.FieldRequiredGroup88](#protobuf-experimental-Proto2Message-FieldRequiredGroup88)
    - [Proto2Message.RequiredNestedMessage](#protobuf-experimental-Proto2Message-RequiredNestedMessage)
    - [Proto2MessageWithExtensions](#protobuf-experimental-Proto2MessageWithExtensions)
    - [Proto2MessageWithMaps](#protobuf-experimental-Proto2MessageWithMaps)
    - [Proto2MessageWithMaps.FieldMapBoolBool1Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolBool1Entry)
    - [Proto2MessageWithMaps.FieldMapBoolBytes2Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolBytes2Entry)
    - [Proto2MessageWithMaps.FieldMapBoolDouble3Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolDouble3Entry)
    - [Proto2MessageWithMaps.FieldMapBoolEnum4Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolEnum4Entry)
    - [Proto2MessageWithMaps.FieldMapBoolFixed325Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFixed325Entry)
    - [Proto2MessageWithMaps.FieldMapBoolFixed646Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFixed646Entry)
    - [Proto2MessageWithMaps.FieldMapBoolFloat7Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFloat7Entry)
    - [Proto2MessageWithMaps.FieldMapBoolInt328Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolInt328Entry)
    - [Proto2MessageWithMaps.FieldMapBoolInt649Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolInt649Entry)
    - [Proto2MessageWithMaps.FieldMapBoolMessage10Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolMessage10Entry)
    - [Proto2MessageWithMaps.FieldMapBoolSfixed3211Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSfixed3211Entry)
    - [Proto2MessageWithMaps.FieldMapBoolSfixed6412Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSfixed6412Entry)
    - [Proto2MessageWithMaps.FieldMapBoolSint3213Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSint3213Entry)
    - [Proto2MessageWithMaps.FieldMapBoolSint6414Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSint6414Entry)
    - [Proto2MessageWithMaps.FieldMapBoolString15Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolString15Entry)
    - [Proto2MessageWithMaps.FieldMapBoolUint3216Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolUint3216Entry)
    - [Proto2MessageWithMaps.FieldMapBoolUint6417Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolUint6417Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Bool18Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Bool18Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Bytes19Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Bytes19Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Double20Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Double20Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Enum21Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Enum21Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Fixed3222Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Fixed3222Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Fixed6423Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Fixed6423Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Float24Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Float24Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Int3225Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Int3225Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Int6426Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Int6426Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Message27Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Message27Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Sfixed3228Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sfixed3228Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Sfixed6429Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sfixed6429Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Sint3230Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sint3230Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Sint6431Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sint6431Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32String32Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32String32Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Uint3233Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Uint3233Entry)
    - [Proto2MessageWithMaps.FieldMapFixed32Uint6434Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Uint6434Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Bool35Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Bool35Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Bytes36Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Bytes36Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Double37Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Double37Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Enum38Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Enum38Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Fixed3239Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Fixed3239Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Fixed6440Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Fixed6440Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Float41Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Float41Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Int3242Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Int3242Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Int6443Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Int6443Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Message44Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Message44Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Sfixed3245Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sfixed3245Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Sfixed6446Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sfixed6446Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Sint3247Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sint3247Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Sint6448Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sint6448Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64String49Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64String49Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Uint3250Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Uint3250Entry)
    - [Proto2MessageWithMaps.FieldMapFixed64Uint6451Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Uint6451Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Bool52Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Bool52Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Bytes53Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Bytes53Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Double54Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Double54Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Enum55Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Enum55Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Fixed3256Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Fixed3256Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Fixed6457Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Fixed6457Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Float58Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Float58Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Int3259Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Int3259Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Int6460Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Int6460Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Message61Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Message61Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Sfixed3262Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sfixed3262Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Sfixed6463Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sfixed6463Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Sint3264Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sint3264Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Sint6465Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sint6465Entry)
    - [Proto2MessageWithMaps.FieldMapInt32String66Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32String66Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Uint3267Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Uint3267Entry)
    - [Proto2MessageWithMaps.FieldMapInt32Uint6468Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Uint6468Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Bool69Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Bool69Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Bytes70Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Bytes70Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Double71Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Double71Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Enum72Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Enum72Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Fixed3273Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Fixed3273Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Fixed6474Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Fixed6474Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Float75Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Float75Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Int3276Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Int3276Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Int6477Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Int6477Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Message78Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Message78Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Sfixed3279Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sfixed3279Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Sfixed6480Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sfixed6480Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Sint3281Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sint3281Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Sint6482Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sint6482Entry)
    - [Proto2MessageWithMaps.FieldMapInt64String83Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64String83Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Uint3284Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Uint3284Entry)
    - [Proto2MessageWithMaps.FieldMapInt64Uint6485Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Uint6485Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Bool86Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Bool86Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Bytes87Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Bytes87Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Double88Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Double88Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Enum89Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Enum89Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Fixed3290Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Fixed3290Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Fixed6491Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Fixed6491Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Float92Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Float92Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Int3293Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Int3293Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Int6494Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Int6494Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Message95Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Message95Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Sfixed3296Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sfixed3296Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Sfixed6497Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sfixed6497Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Sint3298Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sint3298Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Sint6499Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sint6499Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32String100Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32String100Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Uint32101Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Uint32101Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed32Uint64102Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Uint64102Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Bool103Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Bool103Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Bytes104Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Bytes104Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Double105Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Double105Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Enum106Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Enum106Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Fixed32107Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Fixed32107Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Fixed64108Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Fixed64108Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Float109Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Float109Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Int32110Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Int32110Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Int64111Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Int64111Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Message112Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Message112Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Sfixed32113Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sfixed32113Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Sfixed64114Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sfixed64114Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Sint32115Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sint32115Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Sint64116Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sint64116Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64String117Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64String117Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Uint32118Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Uint32118Entry)
    - [Proto2MessageWithMaps.FieldMapSfixed64Uint64119Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Uint64119Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Bool120Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Bool120Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Bytes121Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Bytes121Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Double122Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Double122Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Enum123Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Enum123Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Fixed32124Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Fixed32124Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Fixed64125Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Fixed64125Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Float126Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Float126Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Int32127Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Int32127Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Int64128Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Int64128Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Message129Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Message129Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Sfixed32130Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sfixed32130Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Sfixed64131Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sfixed64131Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Sint32132Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sint32132Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Sint64133Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sint64133Entry)
    - [Proto2MessageWithMaps.FieldMapSint32String134Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32String134Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Uint32135Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Uint32135Entry)
    - [Proto2MessageWithMaps.FieldMapSint32Uint64136Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Uint64136Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Bool137Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Bool137Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Bytes138Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Bytes138Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Double139Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Double139Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Enum140Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Enum140Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Fixed32141Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Fixed32141Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Fixed64142Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Fixed64142Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Float143Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Float143Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Int32144Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Int32144Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Int64145Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Int64145Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Message146Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Message146Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Sfixed32147Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sfixed32147Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Sfixed64148Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sfixed64148Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Sint32149Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sint32149Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Sint64150Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sint64150Entry)
    - [Proto2MessageWithMaps.FieldMapSint64String151Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64String151Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Uint32152Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Uint32152Entry)
    - [Proto2MessageWithMaps.FieldMapSint64Uint64153Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Uint64153Entry)
    - [Proto2MessageWithMaps.FieldMapStringBool154Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringBool154Entry)
    - [Proto2MessageWithMaps.FieldMapStringBytes155Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringBytes155Entry)
    - [Proto2MessageWithMaps.FieldMapStringDouble156Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringDouble156Entry)
    - [Proto2MessageWithMaps.FieldMapStringEnum157Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringEnum157Entry)
    - [Proto2MessageWithMaps.FieldMapStringFixed32158Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFixed32158Entry)
    - [Proto2MessageWithMaps.FieldMapStringFixed64159Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFixed64159Entry)
    - [Proto2MessageWithMaps.FieldMapStringFloat160Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFloat160Entry)
    - [Proto2MessageWithMaps.FieldMapStringInt32161Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringInt32161Entry)
    - [Proto2MessageWithMaps.FieldMapStringInt64162Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringInt64162Entry)
    - [Proto2MessageWithMaps.FieldMapStringMessage163Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringMessage163Entry)
    - [Proto2MessageWithMaps.FieldMapStringSfixed32164Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSfixed32164Entry)
    - [Proto2MessageWithMaps.FieldMapStringSfixed64165Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSfixed64165Entry)
    - [Proto2MessageWithMaps.FieldMapStringSint32166Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSint32166Entry)
    - [Proto2MessageWithMaps.FieldMapStringSint64167Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSint64167Entry)
    - [Proto2MessageWithMaps.FieldMapStringString168Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringString168Entry)
    - [Proto2MessageWithMaps.FieldMapStringUint32169Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringUint32169Entry)
    - [Proto2MessageWithMaps.FieldMapStringUint64170Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringUint64170Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Bool171Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Bool171Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Bytes172Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Bytes172Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Double173Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Double173Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Enum174Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Enum174Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Fixed32175Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Fixed32175Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Fixed64176Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Fixed64176Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Float177Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Float177Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Int32178Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Int32178Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Int64179Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Int64179Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Message180Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Message180Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Sfixed32181Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sfixed32181Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Sfixed64182Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sfixed64182Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Sint32183Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sint32183Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Sint64184Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sint64184Entry)
    - [Proto2MessageWithMaps.FieldMapUint32String185Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32String185Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Uint32186Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Uint32186Entry)
    - [Proto2MessageWithMaps.FieldMapUint32Uint64187Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Uint64187Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Bool188Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Bool188Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Bytes189Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Bytes189Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Double190Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Double190Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Enum191Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Enum191Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Fixed32192Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Fixed32192Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Fixed64193Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Fixed64193Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Float194Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Float194Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Int32195Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Int32195Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Int64196Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Int64196Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Message197Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Message197Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Sfixed32198Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sfixed32198Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Sfixed64199Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sfixed64199Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Sint32200Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sint32200Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Sint64201Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sint64201Entry)
    - [Proto2MessageWithMaps.FieldMapUint64String202Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64String202Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Uint32203Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Uint32203Entry)
    - [Proto2MessageWithMaps.FieldMapUint64Uint64204Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Uint64204Entry)
    - [Proto2SpecialFieldName](#protobuf-experimental-Proto2SpecialFieldName)
  
    - [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum)
  
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
    - [File-level Extensions](#java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_core_src_test_proto_com_google_protobuf_proto2_message-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/core/src/test/proto/com/google/protobuf/proto2_message.proto
LINT: ALLOW_GROUPS


<a name="protobuf-experimental-FieldGroup49"></a>

### FieldGroup49



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_50 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-FieldGroupList51"></a>

### FieldGroupList51



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_52 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2Empty"></a>

### Proto2Empty







<a name="protobuf-experimental-Proto2Message"></a>

### Proto2Message



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
| field_message_10 | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |
| field_bytes_11 | [bytes](#bytes) | optional |  |
| field_uint32_12 | [uint32](#uint32) | optional |  |
| field_enum_13 | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |
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
| field_message_list_27 | [Proto2Message](#protobuf-experimental-Proto2Message) | repeated |  |
| field_bytes_list_28 | [bytes](#bytes) | repeated |  |
| field_uint32_list_29 | [uint32](#uint32) | repeated |  |
| field_enum_list_30 | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | repeated |  |
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
| field_enum_list_packed_44 | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | repeated |  |
| field_sfixed32_list_packed_45 | [sfixed32](#sfixed32) | repeated |  |
| field_sfixed64_list_packed_46 | [sfixed64](#sfixed64) | repeated |  |
| field_sint32_list_packed_47 | [sint32](#sint32) | repeated |  |
| field_sint64_list_packed_48 | [sint64](#sint64) | repeated |  |
| fieldgroup49 | [Proto2Message.FieldGroup49](#protobuf-experimental-Proto2Message-FieldGroup49) | optional |  |
| fieldgrouplist51 | [Proto2Message.FieldGroupList51](#protobuf-experimental-Proto2Message-FieldGroupList51) | repeated |  |
| field_double_53 | [double](#double) | optional |  |
| field_float_54 | [float](#float) | optional |  |
| field_int64_55 | [int64](#int64) | optional |  |
| field_uint64_56 | [uint64](#uint64) | optional |  |
| field_int32_57 | [int32](#int32) | optional |  |
| field_fixed64_58 | [fixed64](#fixed64) | optional |  |
| field_fixed32_59 | [fixed32](#fixed32) | optional |  |
| field_bool_60 | [bool](#bool) | optional |  |
| field_string_61 | [string](#string) | optional |  |
| field_message_62 | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |
| field_bytes_63 | [bytes](#bytes) | optional |  |
| field_uint32_64 | [uint32](#uint32) | optional |  |
| field_sfixed32_65 | [sfixed32](#sfixed32) | optional |  |
| field_sfixed64_66 | [sfixed64](#sfixed64) | optional |  |
| field_sint32_67 | [sint32](#sint32) | optional |  |
| field_sint64_68 | [sint64](#sint64) | optional |  |
| fieldgroup69 | [Proto2Message.FieldGroup69](#protobuf-experimental-Proto2Message-FieldGroup69) | optional |  |
| field_required_double_71 | [double](#double) | required |  |
| field_required_float_72 | [float](#float) | required |  |
| field_required_int64_73 | [int64](#int64) | required |  |
| field_required_uint64_74 | [uint64](#uint64) | required |  |
| field_required_int32_75 | [int32](#int32) | required |  |
| field_required_fixed64_76 | [fixed64](#fixed64) | required |  |
| field_required_fixed32_77 | [fixed32](#fixed32) | required |  |
| field_required_bool_78 | [bool](#bool) | required |  |
| field_required_string_79 | [string](#string) | required |  |
| field_required_message_80 | [Proto2Message.RequiredNestedMessage](#protobuf-experimental-Proto2Message-RequiredNestedMessage) | required |  |
| field_required_bytes_81 | [bytes](#bytes) | required |  |
| field_required_uint32_82 | [uint32](#uint32) | required |  |
| field_required_enum_83 | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | required |  |
| field_required_sfixed32_84 | [sfixed32](#sfixed32) | required |  |
| field_required_sfixed64_85 | [sfixed64](#sfixed64) | required |  |
| field_required_sint32_86 | [sint32](#sint32) | required |  |
| field_required_sint64_87 | [sint64](#sint64) | required |  |
| fieldrequiredgroup88 | [Proto2Message.FieldRequiredGroup88](#protobuf-experimental-Proto2Message-FieldRequiredGroup88) | required |  |






<a name="protobuf-experimental-Proto2Message-FieldGroup49"></a>

### Proto2Message.FieldGroup49



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_50 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2Message-FieldGroup69"></a>

### Proto2Message.FieldGroup69



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_70 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2Message-FieldGroupList51"></a>

### Proto2Message.FieldGroupList51



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_52 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2Message-FieldRequiredGroup88"></a>

### Proto2Message.FieldRequiredGroup88



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_int32_89 | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2Message-RequiredNestedMessage"></a>

### Proto2Message.RequiredNestedMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithExtensions"></a>

### Proto2MessageWithExtensions







<a name="protobuf-experimental-Proto2MessageWithMaps"></a>

### Proto2MessageWithMaps



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_map_bool_bool_1 | [Proto2MessageWithMaps.FieldMapBoolBool1Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolBool1Entry) | repeated |  |
| field_map_bool_bytes_2 | [Proto2MessageWithMaps.FieldMapBoolBytes2Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolBytes2Entry) | repeated |  |
| field_map_bool_double_3 | [Proto2MessageWithMaps.FieldMapBoolDouble3Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolDouble3Entry) | repeated |  |
| field_map_bool_enum_4 | [Proto2MessageWithMaps.FieldMapBoolEnum4Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolEnum4Entry) | repeated |  |
| field_map_bool_fixed32_5 | [Proto2MessageWithMaps.FieldMapBoolFixed325Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFixed325Entry) | repeated |  |
| field_map_bool_fixed64_6 | [Proto2MessageWithMaps.FieldMapBoolFixed646Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFixed646Entry) | repeated |  |
| field_map_bool_float_7 | [Proto2MessageWithMaps.FieldMapBoolFloat7Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFloat7Entry) | repeated |  |
| field_map_bool_int32_8 | [Proto2MessageWithMaps.FieldMapBoolInt328Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolInt328Entry) | repeated |  |
| field_map_bool_int64_9 | [Proto2MessageWithMaps.FieldMapBoolInt649Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolInt649Entry) | repeated |  |
| field_map_bool_message_10 | [Proto2MessageWithMaps.FieldMapBoolMessage10Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolMessage10Entry) | repeated |  |
| field_map_bool_sfixed32_11 | [Proto2MessageWithMaps.FieldMapBoolSfixed3211Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSfixed3211Entry) | repeated |  |
| field_map_bool_sfixed64_12 | [Proto2MessageWithMaps.FieldMapBoolSfixed6412Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSfixed6412Entry) | repeated |  |
| field_map_bool_sint32_13 | [Proto2MessageWithMaps.FieldMapBoolSint3213Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSint3213Entry) | repeated |  |
| field_map_bool_sint64_14 | [Proto2MessageWithMaps.FieldMapBoolSint6414Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSint6414Entry) | repeated |  |
| field_map_bool_string_15 | [Proto2MessageWithMaps.FieldMapBoolString15Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolString15Entry) | repeated |  |
| field_map_bool_uint32_16 | [Proto2MessageWithMaps.FieldMapBoolUint3216Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolUint3216Entry) | repeated |  |
| field_map_bool_uint64_17 | [Proto2MessageWithMaps.FieldMapBoolUint6417Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolUint6417Entry) | repeated |  |
| field_map_fixed32_bool_18 | [Proto2MessageWithMaps.FieldMapFixed32Bool18Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Bool18Entry) | repeated |  |
| field_map_fixed32_bytes_19 | [Proto2MessageWithMaps.FieldMapFixed32Bytes19Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Bytes19Entry) | repeated |  |
| field_map_fixed32_double_20 | [Proto2MessageWithMaps.FieldMapFixed32Double20Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Double20Entry) | repeated |  |
| field_map_fixed32_enum_21 | [Proto2MessageWithMaps.FieldMapFixed32Enum21Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Enum21Entry) | repeated |  |
| field_map_fixed32_fixed32_22 | [Proto2MessageWithMaps.FieldMapFixed32Fixed3222Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Fixed3222Entry) | repeated |  |
| field_map_fixed32_fixed64_23 | [Proto2MessageWithMaps.FieldMapFixed32Fixed6423Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Fixed6423Entry) | repeated |  |
| field_map_fixed32_float_24 | [Proto2MessageWithMaps.FieldMapFixed32Float24Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Float24Entry) | repeated |  |
| field_map_fixed32_int32_25 | [Proto2MessageWithMaps.FieldMapFixed32Int3225Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Int3225Entry) | repeated |  |
| field_map_fixed32_int64_26 | [Proto2MessageWithMaps.FieldMapFixed32Int6426Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Int6426Entry) | repeated |  |
| field_map_fixed32_message_27 | [Proto2MessageWithMaps.FieldMapFixed32Message27Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Message27Entry) | repeated |  |
| field_map_fixed32_sfixed32_28 | [Proto2MessageWithMaps.FieldMapFixed32Sfixed3228Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sfixed3228Entry) | repeated |  |
| field_map_fixed32_sfixed64_29 | [Proto2MessageWithMaps.FieldMapFixed32Sfixed6429Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sfixed6429Entry) | repeated |  |
| field_map_fixed32_sint32_30 | [Proto2MessageWithMaps.FieldMapFixed32Sint3230Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sint3230Entry) | repeated |  |
| field_map_fixed32_sint64_31 | [Proto2MessageWithMaps.FieldMapFixed32Sint6431Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sint6431Entry) | repeated |  |
| field_map_fixed32_string_32 | [Proto2MessageWithMaps.FieldMapFixed32String32Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32String32Entry) | repeated |  |
| field_map_fixed32_uint32_33 | [Proto2MessageWithMaps.FieldMapFixed32Uint3233Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Uint3233Entry) | repeated |  |
| field_map_fixed32_uint64_34 | [Proto2MessageWithMaps.FieldMapFixed32Uint6434Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Uint6434Entry) | repeated |  |
| field_map_fixed64_bool_35 | [Proto2MessageWithMaps.FieldMapFixed64Bool35Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Bool35Entry) | repeated |  |
| field_map_fixed64_bytes_36 | [Proto2MessageWithMaps.FieldMapFixed64Bytes36Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Bytes36Entry) | repeated |  |
| field_map_fixed64_double_37 | [Proto2MessageWithMaps.FieldMapFixed64Double37Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Double37Entry) | repeated |  |
| field_map_fixed64_enum_38 | [Proto2MessageWithMaps.FieldMapFixed64Enum38Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Enum38Entry) | repeated |  |
| field_map_fixed64_fixed32_39 | [Proto2MessageWithMaps.FieldMapFixed64Fixed3239Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Fixed3239Entry) | repeated |  |
| field_map_fixed64_fixed64_40 | [Proto2MessageWithMaps.FieldMapFixed64Fixed6440Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Fixed6440Entry) | repeated |  |
| field_map_fixed64_float_41 | [Proto2MessageWithMaps.FieldMapFixed64Float41Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Float41Entry) | repeated |  |
| field_map_fixed64_int32_42 | [Proto2MessageWithMaps.FieldMapFixed64Int3242Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Int3242Entry) | repeated |  |
| field_map_fixed64_int64_43 | [Proto2MessageWithMaps.FieldMapFixed64Int6443Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Int6443Entry) | repeated |  |
| field_map_fixed64_message_44 | [Proto2MessageWithMaps.FieldMapFixed64Message44Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Message44Entry) | repeated |  |
| field_map_fixed64_sfixed32_45 | [Proto2MessageWithMaps.FieldMapFixed64Sfixed3245Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sfixed3245Entry) | repeated |  |
| field_map_fixed64_sfixed64_46 | [Proto2MessageWithMaps.FieldMapFixed64Sfixed6446Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sfixed6446Entry) | repeated |  |
| field_map_fixed64_sint32_47 | [Proto2MessageWithMaps.FieldMapFixed64Sint3247Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sint3247Entry) | repeated |  |
| field_map_fixed64_sint64_48 | [Proto2MessageWithMaps.FieldMapFixed64Sint6448Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sint6448Entry) | repeated |  |
| field_map_fixed64_string_49 | [Proto2MessageWithMaps.FieldMapFixed64String49Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64String49Entry) | repeated |  |
| field_map_fixed64_uint32_50 | [Proto2MessageWithMaps.FieldMapFixed64Uint3250Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Uint3250Entry) | repeated |  |
| field_map_fixed64_uint64_51 | [Proto2MessageWithMaps.FieldMapFixed64Uint6451Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Uint6451Entry) | repeated |  |
| field_map_int32_bool_52 | [Proto2MessageWithMaps.FieldMapInt32Bool52Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Bool52Entry) | repeated |  |
| field_map_int32_bytes_53 | [Proto2MessageWithMaps.FieldMapInt32Bytes53Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Bytes53Entry) | repeated |  |
| field_map_int32_double_54 | [Proto2MessageWithMaps.FieldMapInt32Double54Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Double54Entry) | repeated |  |
| field_map_int32_enum_55 | [Proto2MessageWithMaps.FieldMapInt32Enum55Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Enum55Entry) | repeated |  |
| field_map_int32_fixed32_56 | [Proto2MessageWithMaps.FieldMapInt32Fixed3256Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Fixed3256Entry) | repeated |  |
| field_map_int32_fixed64_57 | [Proto2MessageWithMaps.FieldMapInt32Fixed6457Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Fixed6457Entry) | repeated |  |
| field_map_int32_float_58 | [Proto2MessageWithMaps.FieldMapInt32Float58Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Float58Entry) | repeated |  |
| field_map_int32_int32_59 | [Proto2MessageWithMaps.FieldMapInt32Int3259Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Int3259Entry) | repeated |  |
| field_map_int32_int64_60 | [Proto2MessageWithMaps.FieldMapInt32Int6460Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Int6460Entry) | repeated |  |
| field_map_int32_message_61 | [Proto2MessageWithMaps.FieldMapInt32Message61Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Message61Entry) | repeated |  |
| field_map_int32_sfixed32_62 | [Proto2MessageWithMaps.FieldMapInt32Sfixed3262Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sfixed3262Entry) | repeated |  |
| field_map_int32_sfixed64_63 | [Proto2MessageWithMaps.FieldMapInt32Sfixed6463Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sfixed6463Entry) | repeated |  |
| field_map_int32_sint32_64 | [Proto2MessageWithMaps.FieldMapInt32Sint3264Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sint3264Entry) | repeated |  |
| field_map_int32_sint64_65 | [Proto2MessageWithMaps.FieldMapInt32Sint6465Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sint6465Entry) | repeated |  |
| field_map_int32_string_66 | [Proto2MessageWithMaps.FieldMapInt32String66Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32String66Entry) | repeated |  |
| field_map_int32_uint32_67 | [Proto2MessageWithMaps.FieldMapInt32Uint3267Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Uint3267Entry) | repeated |  |
| field_map_int32_uint64_68 | [Proto2MessageWithMaps.FieldMapInt32Uint6468Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Uint6468Entry) | repeated |  |
| field_map_int64_bool_69 | [Proto2MessageWithMaps.FieldMapInt64Bool69Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Bool69Entry) | repeated |  |
| field_map_int64_bytes_70 | [Proto2MessageWithMaps.FieldMapInt64Bytes70Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Bytes70Entry) | repeated |  |
| field_map_int64_double_71 | [Proto2MessageWithMaps.FieldMapInt64Double71Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Double71Entry) | repeated |  |
| field_map_int64_enum_72 | [Proto2MessageWithMaps.FieldMapInt64Enum72Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Enum72Entry) | repeated |  |
| field_map_int64_fixed32_73 | [Proto2MessageWithMaps.FieldMapInt64Fixed3273Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Fixed3273Entry) | repeated |  |
| field_map_int64_fixed64_74 | [Proto2MessageWithMaps.FieldMapInt64Fixed6474Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Fixed6474Entry) | repeated |  |
| field_map_int64_float_75 | [Proto2MessageWithMaps.FieldMapInt64Float75Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Float75Entry) | repeated |  |
| field_map_int64_int32_76 | [Proto2MessageWithMaps.FieldMapInt64Int3276Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Int3276Entry) | repeated |  |
| field_map_int64_int64_77 | [Proto2MessageWithMaps.FieldMapInt64Int6477Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Int6477Entry) | repeated |  |
| field_map_int64_message_78 | [Proto2MessageWithMaps.FieldMapInt64Message78Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Message78Entry) | repeated |  |
| field_map_int64_sfixed32_79 | [Proto2MessageWithMaps.FieldMapInt64Sfixed3279Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sfixed3279Entry) | repeated |  |
| field_map_int64_sfixed64_80 | [Proto2MessageWithMaps.FieldMapInt64Sfixed6480Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sfixed6480Entry) | repeated |  |
| field_map_int64_sint32_81 | [Proto2MessageWithMaps.FieldMapInt64Sint3281Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sint3281Entry) | repeated |  |
| field_map_int64_sint64_82 | [Proto2MessageWithMaps.FieldMapInt64Sint6482Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sint6482Entry) | repeated |  |
| field_map_int64_string_83 | [Proto2MessageWithMaps.FieldMapInt64String83Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64String83Entry) | repeated |  |
| field_map_int64_uint32_84 | [Proto2MessageWithMaps.FieldMapInt64Uint3284Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Uint3284Entry) | repeated |  |
| field_map_int64_uint64_85 | [Proto2MessageWithMaps.FieldMapInt64Uint6485Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Uint6485Entry) | repeated |  |
| field_map_sfixed32_bool_86 | [Proto2MessageWithMaps.FieldMapSfixed32Bool86Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Bool86Entry) | repeated |  |
| field_map_sfixed32_bytes_87 | [Proto2MessageWithMaps.FieldMapSfixed32Bytes87Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Bytes87Entry) | repeated |  |
| field_map_sfixed32_double_88 | [Proto2MessageWithMaps.FieldMapSfixed32Double88Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Double88Entry) | repeated |  |
| field_map_sfixed32_enum_89 | [Proto2MessageWithMaps.FieldMapSfixed32Enum89Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Enum89Entry) | repeated |  |
| field_map_sfixed32_fixed32_90 | [Proto2MessageWithMaps.FieldMapSfixed32Fixed3290Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Fixed3290Entry) | repeated |  |
| field_map_sfixed32_fixed64_91 | [Proto2MessageWithMaps.FieldMapSfixed32Fixed6491Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Fixed6491Entry) | repeated |  |
| field_map_sfixed32_float_92 | [Proto2MessageWithMaps.FieldMapSfixed32Float92Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Float92Entry) | repeated |  |
| field_map_sfixed32_int32_93 | [Proto2MessageWithMaps.FieldMapSfixed32Int3293Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Int3293Entry) | repeated |  |
| field_map_sfixed32_int64_94 | [Proto2MessageWithMaps.FieldMapSfixed32Int6494Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Int6494Entry) | repeated |  |
| field_map_sfixed32_message_95 | [Proto2MessageWithMaps.FieldMapSfixed32Message95Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Message95Entry) | repeated |  |
| field_map_sfixed32_sfixed32_96 | [Proto2MessageWithMaps.FieldMapSfixed32Sfixed3296Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sfixed3296Entry) | repeated |  |
| field_map_sfixed32_sfixed64_97 | [Proto2MessageWithMaps.FieldMapSfixed32Sfixed6497Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sfixed6497Entry) | repeated |  |
| field_map_sfixed32_sint32_98 | [Proto2MessageWithMaps.FieldMapSfixed32Sint3298Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sint3298Entry) | repeated |  |
| field_map_sfixed32_sint64_99 | [Proto2MessageWithMaps.FieldMapSfixed32Sint6499Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sint6499Entry) | repeated |  |
| field_map_sfixed32_string_100 | [Proto2MessageWithMaps.FieldMapSfixed32String100Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32String100Entry) | repeated |  |
| field_map_sfixed32_uint32_101 | [Proto2MessageWithMaps.FieldMapSfixed32Uint32101Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Uint32101Entry) | repeated |  |
| field_map_sfixed32_uint64_102 | [Proto2MessageWithMaps.FieldMapSfixed32Uint64102Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Uint64102Entry) | repeated |  |
| field_map_sfixed64_bool_103 | [Proto2MessageWithMaps.FieldMapSfixed64Bool103Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Bool103Entry) | repeated |  |
| field_map_sfixed64_bytes_104 | [Proto2MessageWithMaps.FieldMapSfixed64Bytes104Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Bytes104Entry) | repeated |  |
| field_map_sfixed64_double_105 | [Proto2MessageWithMaps.FieldMapSfixed64Double105Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Double105Entry) | repeated |  |
| field_map_sfixed64_enum_106 | [Proto2MessageWithMaps.FieldMapSfixed64Enum106Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Enum106Entry) | repeated |  |
| field_map_sfixed64_fixed32_107 | [Proto2MessageWithMaps.FieldMapSfixed64Fixed32107Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Fixed32107Entry) | repeated |  |
| field_map_sfixed64_fixed64_108 | [Proto2MessageWithMaps.FieldMapSfixed64Fixed64108Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Fixed64108Entry) | repeated |  |
| field_map_sfixed64_float_109 | [Proto2MessageWithMaps.FieldMapSfixed64Float109Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Float109Entry) | repeated |  |
| field_map_sfixed64_int32_110 | [Proto2MessageWithMaps.FieldMapSfixed64Int32110Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Int32110Entry) | repeated |  |
| field_map_sfixed64_int64_111 | [Proto2MessageWithMaps.FieldMapSfixed64Int64111Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Int64111Entry) | repeated |  |
| field_map_sfixed64_message_112 | [Proto2MessageWithMaps.FieldMapSfixed64Message112Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Message112Entry) | repeated |  |
| field_map_sfixed64_sfixed32_113 | [Proto2MessageWithMaps.FieldMapSfixed64Sfixed32113Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sfixed32113Entry) | repeated |  |
| field_map_sfixed64_sfixed64_114 | [Proto2MessageWithMaps.FieldMapSfixed64Sfixed64114Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sfixed64114Entry) | repeated |  |
| field_map_sfixed64_sint32_115 | [Proto2MessageWithMaps.FieldMapSfixed64Sint32115Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sint32115Entry) | repeated |  |
| field_map_sfixed64_sint64_116 | [Proto2MessageWithMaps.FieldMapSfixed64Sint64116Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sint64116Entry) | repeated |  |
| field_map_sfixed64_string_117 | [Proto2MessageWithMaps.FieldMapSfixed64String117Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64String117Entry) | repeated |  |
| field_map_sfixed64_uint32_118 | [Proto2MessageWithMaps.FieldMapSfixed64Uint32118Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Uint32118Entry) | repeated |  |
| field_map_sfixed64_uint64_119 | [Proto2MessageWithMaps.FieldMapSfixed64Uint64119Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Uint64119Entry) | repeated |  |
| field_map_sint32_bool_120 | [Proto2MessageWithMaps.FieldMapSint32Bool120Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Bool120Entry) | repeated |  |
| field_map_sint32_bytes_121 | [Proto2MessageWithMaps.FieldMapSint32Bytes121Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Bytes121Entry) | repeated |  |
| field_map_sint32_double_122 | [Proto2MessageWithMaps.FieldMapSint32Double122Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Double122Entry) | repeated |  |
| field_map_sint32_enum_123 | [Proto2MessageWithMaps.FieldMapSint32Enum123Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Enum123Entry) | repeated |  |
| field_map_sint32_fixed32_124 | [Proto2MessageWithMaps.FieldMapSint32Fixed32124Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Fixed32124Entry) | repeated |  |
| field_map_sint32_fixed64_125 | [Proto2MessageWithMaps.FieldMapSint32Fixed64125Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Fixed64125Entry) | repeated |  |
| field_map_sint32_float_126 | [Proto2MessageWithMaps.FieldMapSint32Float126Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Float126Entry) | repeated |  |
| field_map_sint32_int32_127 | [Proto2MessageWithMaps.FieldMapSint32Int32127Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Int32127Entry) | repeated |  |
| field_map_sint32_int64_128 | [Proto2MessageWithMaps.FieldMapSint32Int64128Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Int64128Entry) | repeated |  |
| field_map_sint32_message_129 | [Proto2MessageWithMaps.FieldMapSint32Message129Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Message129Entry) | repeated |  |
| field_map_sint32_sfixed32_130 | [Proto2MessageWithMaps.FieldMapSint32Sfixed32130Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sfixed32130Entry) | repeated |  |
| field_map_sint32_sfixed64_131 | [Proto2MessageWithMaps.FieldMapSint32Sfixed64131Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sfixed64131Entry) | repeated |  |
| field_map_sint32_sint32_132 | [Proto2MessageWithMaps.FieldMapSint32Sint32132Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sint32132Entry) | repeated |  |
| field_map_sint32_sint64_133 | [Proto2MessageWithMaps.FieldMapSint32Sint64133Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sint64133Entry) | repeated |  |
| field_map_sint32_string_134 | [Proto2MessageWithMaps.FieldMapSint32String134Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32String134Entry) | repeated |  |
| field_map_sint32_uint32_135 | [Proto2MessageWithMaps.FieldMapSint32Uint32135Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Uint32135Entry) | repeated |  |
| field_map_sint32_uint64_136 | [Proto2MessageWithMaps.FieldMapSint32Uint64136Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Uint64136Entry) | repeated |  |
| field_map_sint64_bool_137 | [Proto2MessageWithMaps.FieldMapSint64Bool137Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Bool137Entry) | repeated |  |
| field_map_sint64_bytes_138 | [Proto2MessageWithMaps.FieldMapSint64Bytes138Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Bytes138Entry) | repeated |  |
| field_map_sint64_double_139 | [Proto2MessageWithMaps.FieldMapSint64Double139Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Double139Entry) | repeated |  |
| field_map_sint64_enum_140 | [Proto2MessageWithMaps.FieldMapSint64Enum140Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Enum140Entry) | repeated |  |
| field_map_sint64_fixed32_141 | [Proto2MessageWithMaps.FieldMapSint64Fixed32141Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Fixed32141Entry) | repeated |  |
| field_map_sint64_fixed64_142 | [Proto2MessageWithMaps.FieldMapSint64Fixed64142Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Fixed64142Entry) | repeated |  |
| field_map_sint64_float_143 | [Proto2MessageWithMaps.FieldMapSint64Float143Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Float143Entry) | repeated |  |
| field_map_sint64_int32_144 | [Proto2MessageWithMaps.FieldMapSint64Int32144Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Int32144Entry) | repeated |  |
| field_map_sint64_int64_145 | [Proto2MessageWithMaps.FieldMapSint64Int64145Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Int64145Entry) | repeated |  |
| field_map_sint64_message_146 | [Proto2MessageWithMaps.FieldMapSint64Message146Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Message146Entry) | repeated |  |
| field_map_sint64_sfixed32_147 | [Proto2MessageWithMaps.FieldMapSint64Sfixed32147Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sfixed32147Entry) | repeated |  |
| field_map_sint64_sfixed64_148 | [Proto2MessageWithMaps.FieldMapSint64Sfixed64148Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sfixed64148Entry) | repeated |  |
| field_map_sint64_sint32_149 | [Proto2MessageWithMaps.FieldMapSint64Sint32149Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sint32149Entry) | repeated |  |
| field_map_sint64_sint64_150 | [Proto2MessageWithMaps.FieldMapSint64Sint64150Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sint64150Entry) | repeated |  |
| field_map_sint64_string_151 | [Proto2MessageWithMaps.FieldMapSint64String151Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64String151Entry) | repeated |  |
| field_map_sint64_uint32_152 | [Proto2MessageWithMaps.FieldMapSint64Uint32152Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Uint32152Entry) | repeated |  |
| field_map_sint64_uint64_153 | [Proto2MessageWithMaps.FieldMapSint64Uint64153Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Uint64153Entry) | repeated |  |
| field_map_string_bool_154 | [Proto2MessageWithMaps.FieldMapStringBool154Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringBool154Entry) | repeated |  |
| field_map_string_bytes_155 | [Proto2MessageWithMaps.FieldMapStringBytes155Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringBytes155Entry) | repeated |  |
| field_map_string_double_156 | [Proto2MessageWithMaps.FieldMapStringDouble156Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringDouble156Entry) | repeated |  |
| field_map_string_enum_157 | [Proto2MessageWithMaps.FieldMapStringEnum157Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringEnum157Entry) | repeated |  |
| field_map_string_fixed32_158 | [Proto2MessageWithMaps.FieldMapStringFixed32158Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFixed32158Entry) | repeated |  |
| field_map_string_fixed64_159 | [Proto2MessageWithMaps.FieldMapStringFixed64159Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFixed64159Entry) | repeated |  |
| field_map_string_float_160 | [Proto2MessageWithMaps.FieldMapStringFloat160Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFloat160Entry) | repeated |  |
| field_map_string_int32_161 | [Proto2MessageWithMaps.FieldMapStringInt32161Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringInt32161Entry) | repeated |  |
| field_map_string_int64_162 | [Proto2MessageWithMaps.FieldMapStringInt64162Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringInt64162Entry) | repeated |  |
| field_map_string_message_163 | [Proto2MessageWithMaps.FieldMapStringMessage163Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringMessage163Entry) | repeated |  |
| field_map_string_sfixed32_164 | [Proto2MessageWithMaps.FieldMapStringSfixed32164Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSfixed32164Entry) | repeated |  |
| field_map_string_sfixed64_165 | [Proto2MessageWithMaps.FieldMapStringSfixed64165Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSfixed64165Entry) | repeated |  |
| field_map_string_sint32_166 | [Proto2MessageWithMaps.FieldMapStringSint32166Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSint32166Entry) | repeated |  |
| field_map_string_sint64_167 | [Proto2MessageWithMaps.FieldMapStringSint64167Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSint64167Entry) | repeated |  |
| field_map_string_string_168 | [Proto2MessageWithMaps.FieldMapStringString168Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringString168Entry) | repeated |  |
| field_map_string_uint32_169 | [Proto2MessageWithMaps.FieldMapStringUint32169Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringUint32169Entry) | repeated |  |
| field_map_string_uint64_170 | [Proto2MessageWithMaps.FieldMapStringUint64170Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapStringUint64170Entry) | repeated |  |
| field_map_uint32_bool_171 | [Proto2MessageWithMaps.FieldMapUint32Bool171Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Bool171Entry) | repeated |  |
| field_map_uint32_bytes_172 | [Proto2MessageWithMaps.FieldMapUint32Bytes172Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Bytes172Entry) | repeated |  |
| field_map_uint32_double_173 | [Proto2MessageWithMaps.FieldMapUint32Double173Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Double173Entry) | repeated |  |
| field_map_uint32_enum_174 | [Proto2MessageWithMaps.FieldMapUint32Enum174Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Enum174Entry) | repeated |  |
| field_map_uint32_fixed32_175 | [Proto2MessageWithMaps.FieldMapUint32Fixed32175Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Fixed32175Entry) | repeated |  |
| field_map_uint32_fixed64_176 | [Proto2MessageWithMaps.FieldMapUint32Fixed64176Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Fixed64176Entry) | repeated |  |
| field_map_uint32_float_177 | [Proto2MessageWithMaps.FieldMapUint32Float177Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Float177Entry) | repeated |  |
| field_map_uint32_int32_178 | [Proto2MessageWithMaps.FieldMapUint32Int32178Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Int32178Entry) | repeated |  |
| field_map_uint32_int64_179 | [Proto2MessageWithMaps.FieldMapUint32Int64179Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Int64179Entry) | repeated |  |
| field_map_uint32_message_180 | [Proto2MessageWithMaps.FieldMapUint32Message180Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Message180Entry) | repeated |  |
| field_map_uint32_sfixed32_181 | [Proto2MessageWithMaps.FieldMapUint32Sfixed32181Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sfixed32181Entry) | repeated |  |
| field_map_uint32_sfixed64_182 | [Proto2MessageWithMaps.FieldMapUint32Sfixed64182Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sfixed64182Entry) | repeated |  |
| field_map_uint32_sint32_183 | [Proto2MessageWithMaps.FieldMapUint32Sint32183Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sint32183Entry) | repeated |  |
| field_map_uint32_sint64_184 | [Proto2MessageWithMaps.FieldMapUint32Sint64184Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sint64184Entry) | repeated |  |
| field_map_uint32_string_185 | [Proto2MessageWithMaps.FieldMapUint32String185Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32String185Entry) | repeated |  |
| field_map_uint32_uint32_186 | [Proto2MessageWithMaps.FieldMapUint32Uint32186Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Uint32186Entry) | repeated |  |
| field_map_uint32_uint64_187 | [Proto2MessageWithMaps.FieldMapUint32Uint64187Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Uint64187Entry) | repeated |  |
| field_map_uint64_bool_188 | [Proto2MessageWithMaps.FieldMapUint64Bool188Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Bool188Entry) | repeated |  |
| field_map_uint64_bytes_189 | [Proto2MessageWithMaps.FieldMapUint64Bytes189Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Bytes189Entry) | repeated |  |
| field_map_uint64_double_190 | [Proto2MessageWithMaps.FieldMapUint64Double190Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Double190Entry) | repeated |  |
| field_map_uint64_enum_191 | [Proto2MessageWithMaps.FieldMapUint64Enum191Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Enum191Entry) | repeated |  |
| field_map_uint64_fixed32_192 | [Proto2MessageWithMaps.FieldMapUint64Fixed32192Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Fixed32192Entry) | repeated |  |
| field_map_uint64_fixed64_193 | [Proto2MessageWithMaps.FieldMapUint64Fixed64193Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Fixed64193Entry) | repeated |  |
| field_map_uint64_float_194 | [Proto2MessageWithMaps.FieldMapUint64Float194Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Float194Entry) | repeated |  |
| field_map_uint64_int32_195 | [Proto2MessageWithMaps.FieldMapUint64Int32195Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Int32195Entry) | repeated |  |
| field_map_uint64_int64_196 | [Proto2MessageWithMaps.FieldMapUint64Int64196Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Int64196Entry) | repeated |  |
| field_map_uint64_message_197 | [Proto2MessageWithMaps.FieldMapUint64Message197Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Message197Entry) | repeated |  |
| field_map_uint64_sfixed32_198 | [Proto2MessageWithMaps.FieldMapUint64Sfixed32198Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sfixed32198Entry) | repeated |  |
| field_map_uint64_sfixed64_199 | [Proto2MessageWithMaps.FieldMapUint64Sfixed64199Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sfixed64199Entry) | repeated |  |
| field_map_uint64_sint32_200 | [Proto2MessageWithMaps.FieldMapUint64Sint32200Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sint32200Entry) | repeated |  |
| field_map_uint64_sint64_201 | [Proto2MessageWithMaps.FieldMapUint64Sint64201Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sint64201Entry) | repeated |  |
| field_map_uint64_string_202 | [Proto2MessageWithMaps.FieldMapUint64String202Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64String202Entry) | repeated |  |
| field_map_uint64_uint32_203 | [Proto2MessageWithMaps.FieldMapUint64Uint32203Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Uint32203Entry) | repeated |  |
| field_map_uint64_uint64_204 | [Proto2MessageWithMaps.FieldMapUint64Uint64204Entry](#protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Uint64204Entry) | repeated |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolBool1Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolBool1Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolBytes2Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolBytes2Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolDouble3Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolDouble3Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolEnum4Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolEnum4Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFixed325Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolFixed325Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFixed646Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolFixed646Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolFloat7Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolFloat7Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolInt328Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolInt328Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolInt649Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolInt649Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolMessage10Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolMessage10Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSfixed3211Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolSfixed3211Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSfixed6412Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolSfixed6412Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSint3213Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolSint3213Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolSint6414Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolSint6414Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolString15Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolString15Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolUint3216Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolUint3216Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapBoolUint6417Entry"></a>

### Proto2MessageWithMaps.FieldMapBoolUint6417Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Bool18Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Bool18Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Bytes19Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Bytes19Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Double20Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Double20Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Enum21Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Enum21Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Fixed3222Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Fixed3222Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Fixed6423Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Fixed6423Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Float24Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Float24Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Int3225Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Int3225Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Int6426Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Int6426Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Message27Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Message27Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sfixed3228Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Sfixed3228Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sfixed6429Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Sfixed6429Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sint3230Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Sint3230Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Sint6431Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Sint6431Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32String32Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32String32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Uint3233Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Uint3233Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed32Uint6434Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed32Uint6434Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Bool35Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Bool35Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Bytes36Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Bytes36Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Double37Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Double37Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Enum38Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Enum38Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Fixed3239Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Fixed3239Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Fixed6440Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Fixed6440Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Float41Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Float41Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Int3242Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Int3242Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Int6443Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Int6443Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Message44Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Message44Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sfixed3245Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Sfixed3245Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sfixed6446Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Sfixed6446Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sint3247Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Sint3247Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Sint6448Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Sint6448Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64String49Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64String49Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Uint3250Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Uint3250Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapFixed64Uint6451Entry"></a>

### Proto2MessageWithMaps.FieldMapFixed64Uint6451Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Bool52Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Bool52Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Bytes53Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Bytes53Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Double54Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Double54Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Enum55Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Enum55Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Fixed3256Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Fixed3256Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Fixed6457Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Fixed6457Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Float58Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Float58Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Int3259Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Int3259Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Int6460Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Int6460Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Message61Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Message61Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sfixed3262Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Sfixed3262Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sfixed6463Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Sfixed6463Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sint3264Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Sint3264Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Sint6465Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Sint6465Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32String66Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32String66Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Uint3267Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Uint3267Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt32Uint6468Entry"></a>

### Proto2MessageWithMaps.FieldMapInt32Uint6468Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Bool69Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Bool69Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Bytes70Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Bytes70Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Double71Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Double71Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Enum72Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Enum72Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Fixed3273Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Fixed3273Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Fixed6474Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Fixed6474Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Float75Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Float75Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Int3276Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Int3276Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Int6477Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Int6477Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Message78Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Message78Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sfixed3279Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Sfixed3279Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sfixed6480Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Sfixed6480Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sint3281Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Sint3281Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Sint6482Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Sint6482Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64String83Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64String83Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Uint3284Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Uint3284Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapInt64Uint6485Entry"></a>

### Proto2MessageWithMaps.FieldMapInt64Uint6485Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Bool86Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Bool86Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Bytes87Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Bytes87Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Double88Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Double88Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Enum89Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Enum89Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Fixed3290Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Fixed3290Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Fixed6491Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Fixed6491Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Float92Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Float92Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Int3293Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Int3293Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Int6494Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Int6494Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Message95Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Message95Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sfixed3296Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Sfixed3296Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sfixed6497Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Sfixed6497Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sint3298Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Sint3298Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Sint6499Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Sint6499Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32String100Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32String100Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Uint32101Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Uint32101Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed32Uint64102Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed32Uint64102Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Bool103Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Bool103Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Bytes104Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Bytes104Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Double105Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Double105Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Enum106Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Enum106Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Fixed32107Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Fixed32107Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Fixed64108Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Fixed64108Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Float109Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Float109Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Int32110Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Int32110Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Int64111Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Int64111Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Message112Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Message112Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sfixed32113Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Sfixed32113Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sfixed64114Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Sfixed64114Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sint32115Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Sint32115Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Sint64116Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Sint64116Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64String117Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64String117Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Uint32118Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Uint32118Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSfixed64Uint64119Entry"></a>

### Proto2MessageWithMaps.FieldMapSfixed64Uint64119Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Bool120Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Bool120Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Bytes121Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Bytes121Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Double122Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Double122Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Enum123Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Enum123Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Fixed32124Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Fixed32124Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Fixed64125Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Fixed64125Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Float126Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Float126Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Int32127Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Int32127Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Int64128Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Int64128Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Message129Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Message129Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sfixed32130Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Sfixed32130Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sfixed64131Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Sfixed64131Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sint32132Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Sint32132Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Sint64133Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Sint64133Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32String134Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32String134Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Uint32135Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Uint32135Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint32Uint64136Entry"></a>

### Proto2MessageWithMaps.FieldMapSint32Uint64136Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Bool137Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Bool137Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Bytes138Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Bytes138Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Double139Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Double139Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Enum140Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Enum140Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Fixed32141Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Fixed32141Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Fixed64142Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Fixed64142Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Float143Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Float143Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Int32144Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Int32144Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Int64145Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Int64145Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Message146Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Message146Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sfixed32147Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Sfixed32147Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sfixed64148Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Sfixed64148Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sint32149Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Sint32149Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Sint64150Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Sint64150Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64String151Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64String151Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Uint32152Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Uint32152Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapSint64Uint64153Entry"></a>

### Proto2MessageWithMaps.FieldMapSint64Uint64153Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringBool154Entry"></a>

### Proto2MessageWithMaps.FieldMapStringBool154Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringBytes155Entry"></a>

### Proto2MessageWithMaps.FieldMapStringBytes155Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringDouble156Entry"></a>

### Proto2MessageWithMaps.FieldMapStringDouble156Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringEnum157Entry"></a>

### Proto2MessageWithMaps.FieldMapStringEnum157Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFixed32158Entry"></a>

### Proto2MessageWithMaps.FieldMapStringFixed32158Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFixed64159Entry"></a>

### Proto2MessageWithMaps.FieldMapStringFixed64159Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringFloat160Entry"></a>

### Proto2MessageWithMaps.FieldMapStringFloat160Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringInt32161Entry"></a>

### Proto2MessageWithMaps.FieldMapStringInt32161Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringInt64162Entry"></a>

### Proto2MessageWithMaps.FieldMapStringInt64162Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringMessage163Entry"></a>

### Proto2MessageWithMaps.FieldMapStringMessage163Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSfixed32164Entry"></a>

### Proto2MessageWithMaps.FieldMapStringSfixed32164Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSfixed64165Entry"></a>

### Proto2MessageWithMaps.FieldMapStringSfixed64165Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSint32166Entry"></a>

### Proto2MessageWithMaps.FieldMapStringSint32166Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringSint64167Entry"></a>

### Proto2MessageWithMaps.FieldMapStringSint64167Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringString168Entry"></a>

### Proto2MessageWithMaps.FieldMapStringString168Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringUint32169Entry"></a>

### Proto2MessageWithMaps.FieldMapStringUint32169Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapStringUint64170Entry"></a>

### Proto2MessageWithMaps.FieldMapStringUint64170Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Bool171Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Bool171Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Bytes172Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Bytes172Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Double173Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Double173Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Enum174Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Enum174Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Fixed32175Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Fixed32175Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Fixed64176Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Fixed64176Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Float177Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Float177Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Int32178Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Int32178Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Int64179Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Int64179Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Message180Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Message180Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sfixed32181Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Sfixed32181Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sfixed64182Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Sfixed64182Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sint32183Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Sint32183Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Sint64184Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Sint64184Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32String185Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32String185Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Uint32186Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Uint32186Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint32Uint64187Entry"></a>

### Proto2MessageWithMaps.FieldMapUint32Uint64187Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Bool188Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Bool188Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [bool](#bool) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Bytes189Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Bytes189Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [bytes](#bytes) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Double190Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Double190Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [double](#double) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Enum191Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Enum191Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [Proto2Message.TestEnum](#protobuf-experimental-Proto2Message-TestEnum) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Fixed32192Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Fixed32192Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [fixed32](#fixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Fixed64193Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Fixed64193Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [fixed64](#fixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Float194Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Float194Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [float](#float) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Int32195Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Int32195Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [int32](#int32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Int64196Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Int64196Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [int64](#int64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Message197Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Message197Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [Proto2Message](#protobuf-experimental-Proto2Message) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sfixed32198Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Sfixed32198Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sfixed32](#sfixed32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sfixed64199Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Sfixed64199Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sfixed64](#sfixed64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sint32200Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Sint32200Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sint32](#sint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Sint64201Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Sint64201Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [sint64](#sint64) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64String202Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64String202Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [string](#string) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Uint32203Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Uint32203Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [uint32](#uint32) | optional |  |






<a name="protobuf-experimental-Proto2MessageWithMaps-FieldMapUint64Uint64204Entry"></a>

### Proto2MessageWithMaps.FieldMapUint64Uint64204Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) | optional |  |
| value | [uint64](#uint64) | optional |  |






<a name="protobuf-experimental-Proto2SpecialFieldName"></a>

### Proto2SpecialFieldName



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| regular_name | [double](#double) | optional |  |
| cached_size | [int32](#int32) | optional |  |
| serialized_size | [int64](#int64) | optional |  |
| class | [string](#string) | optional |  |





 


<a name="protobuf-experimental-Proto2Message-TestEnum"></a>

### Proto2Message.TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |
| TWO | 2 |  |


 


<a name="java_core_src_test_proto_com_google_protobuf_proto2_message-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| field_bool_8 | bool | Proto2MessageWithExtensions | 8 |  |
| field_bool_list_25 | bool | Proto2MessageWithExtensions | 25 |  |
| field_bool_list_packed_42 | bool | Proto2MessageWithExtensions | 42 |  |
| field_bytes_11 | bytes | Proto2MessageWithExtensions | 11 |  |
| field_bytes_list_28 | bytes | Proto2MessageWithExtensions | 28 |  |
| field_double_1 | double | Proto2MessageWithExtensions | 1 |  |
| field_double_list_18 | double | Proto2MessageWithExtensions | 18 |  |
| field_double_list_packed_35 | double | Proto2MessageWithExtensions | 35 |  |
| field_enum_13 | Proto2Message.TestEnum | Proto2MessageWithExtensions | 13 |  |
| field_enum_list_30 | Proto2Message.TestEnum | Proto2MessageWithExtensions | 30 |  |
| field_enum_list_packed_44 | Proto2Message.TestEnum | Proto2MessageWithExtensions | 44 |  |
| field_fixed32_7 | fixed32 | Proto2MessageWithExtensions | 7 |  |
| field_fixed32_list_24 | fixed32 | Proto2MessageWithExtensions | 24 |  |
| field_fixed32_list_packed_41 | fixed32 | Proto2MessageWithExtensions | 41 |  |
| field_fixed64_6 | fixed64 | Proto2MessageWithExtensions | 6 |  |
| field_fixed64_list_23 | fixed64 | Proto2MessageWithExtensions | 23 |  |
| field_fixed64_list_packed_40 | fixed64 | Proto2MessageWithExtensions | 40 |  |
| field_float_2 | float | Proto2MessageWithExtensions | 2 |  |
| field_float_list_19 | float | Proto2MessageWithExtensions | 19 |  |
| field_float_list_packed_36 | float | Proto2MessageWithExtensions | 36 |  |
| field_int32_5 | int32 | Proto2MessageWithExtensions | 5 |  |
| field_int32_list_22 | int32 | Proto2MessageWithExtensions | 22 |  |
| field_int32_list_packed_39 | int32 | Proto2MessageWithExtensions | 39 |  |
| field_int64_3 | int64 | Proto2MessageWithExtensions | 3 |  |
| field_int64_list_20 | int64 | Proto2MessageWithExtensions | 20 |  |
| field_int64_list_packed_37 | int64 | Proto2MessageWithExtensions | 37 |  |
| field_message_10 | Proto2Message | Proto2MessageWithExtensions | 10 |  |
| field_message_list_27 | Proto2Message | Proto2MessageWithExtensions | 27 |  |
| field_sfixed32_14 | sfixed32 | Proto2MessageWithExtensions | 14 |  |
| field_sfixed32_list_31 | sfixed32 | Proto2MessageWithExtensions | 31 |  |
| field_sfixed32_list_packed_45 | sfixed32 | Proto2MessageWithExtensions | 45 |  |
| field_sfixed64_15 | sfixed64 | Proto2MessageWithExtensions | 15 |  |
| field_sfixed64_list_32 | sfixed64 | Proto2MessageWithExtensions | 32 |  |
| field_sfixed64_list_packed_46 | sfixed64 | Proto2MessageWithExtensions | 46 |  |
| field_sint32_16 | sint32 | Proto2MessageWithExtensions | 16 |  |
| field_sint32_list_33 | sint32 | Proto2MessageWithExtensions | 33 |  |
| field_sint32_list_packed_47 | sint32 | Proto2MessageWithExtensions | 47 |  |
| field_sint64_17 | sint64 | Proto2MessageWithExtensions | 17 |  |
| field_sint64_list_34 | sint64 | Proto2MessageWithExtensions | 34 |  |
| field_sint64_list_packed_48 | sint64 | Proto2MessageWithExtensions | 48 |  |
| field_string_9 | string | Proto2MessageWithExtensions | 9 |  |
| field_string_list_26 | string | Proto2MessageWithExtensions | 26 |  |
| field_uint32_12 | uint32 | Proto2MessageWithExtensions | 12 |  |
| field_uint32_list_29 | uint32 | Proto2MessageWithExtensions | 29 |  |
| field_uint32_list_packed_43 | uint32 | Proto2MessageWithExtensions | 43 |  |
| field_uint64_4 | uint64 | Proto2MessageWithExtensions | 4 |  |
| field_uint64_list_21 | uint64 | Proto2MessageWithExtensions | 21 |  |
| field_uint64_list_packed_38 | uint64 | Proto2MessageWithExtensions | 38 |  |
| fieldgroup49 | FieldGroup49 | Proto2MessageWithExtensions | 49 |  |
| fieldgrouplist51 | FieldGroupList51 | Proto2MessageWithExtensions | 51 |  |

 

 



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

