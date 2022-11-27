# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [java/core/src/test/proto/com/google/protobuf/proto3_message_lite.proto](#java_core_src_test_proto_com_google_protobuf_proto3_message_lite-proto)
    - [Proto3EmptyLite](#protobuf-experimental-Proto3EmptyLite)
    - [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite)
    - [Proto3MessageLiteWithMaps](#protobuf-experimental-Proto3MessageLiteWithMaps)
    - [Proto3MessageLiteWithMaps.FieldMapBoolBool1Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolBool1Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolBytes2Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolBytes2Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolDouble3Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolDouble3Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolEnum4Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolEnum4Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolFixed325Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFixed325Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolFixed646Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFixed646Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolFloat7Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFloat7Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolInt328Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolInt328Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolInt649Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolInt649Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolMessage10Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolMessage10Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolSfixed3211Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSfixed3211Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolSfixed6412Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSfixed6412Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolSint3213Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSint3213Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolSint6414Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSint6414Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolString15Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolString15Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolUint3216Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolUint3216Entry)
    - [Proto3MessageLiteWithMaps.FieldMapBoolUint6417Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolUint6417Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Bool18Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Bool18Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Bytes19Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Bytes19Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Double20Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Double20Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Enum21Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Enum21Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Fixed3222Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Fixed3222Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Fixed6423Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Fixed6423Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Float24Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Float24Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Int3225Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Int3225Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Int6426Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Int6426Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Message27Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Message27Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Sfixed3228Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sfixed3228Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Sfixed6429Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sfixed6429Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Sint3230Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sint3230Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Sint6431Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sint6431Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32String32Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32String32Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Uint3233Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Uint3233Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed32Uint6434Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Uint6434Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Bool35Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Bool35Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Bytes36Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Bytes36Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Double37Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Double37Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Enum38Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Enum38Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Fixed3239Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Fixed3239Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Fixed6440Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Fixed6440Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Float41Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Float41Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Int3242Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Int3242Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Int6443Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Int6443Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Message44Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Message44Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Sfixed3245Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sfixed3245Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Sfixed6446Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sfixed6446Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Sint3247Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sint3247Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Sint6448Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sint6448Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64String49Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64String49Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Uint3250Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Uint3250Entry)
    - [Proto3MessageLiteWithMaps.FieldMapFixed64Uint6451Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Uint6451Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Bool52Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Bool52Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Bytes53Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Bytes53Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Double54Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Double54Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Enum55Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Enum55Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Fixed3256Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Fixed3256Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Fixed6457Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Fixed6457Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Float58Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Float58Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Int3259Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Int3259Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Int6460Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Int6460Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Message61Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Message61Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Sfixed3262Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sfixed3262Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Sfixed6463Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sfixed6463Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Sint3264Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sint3264Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Sint6465Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sint6465Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32String66Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32String66Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Uint3267Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Uint3267Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt32Uint6468Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Uint6468Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Bool69Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Bool69Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Bytes70Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Bytes70Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Double71Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Double71Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Enum72Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Enum72Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Fixed3273Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Fixed3273Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Fixed6474Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Fixed6474Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Float75Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Float75Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Int3276Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Int3276Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Int6477Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Int6477Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Message78Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Message78Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Sfixed3279Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sfixed3279Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Sfixed6480Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sfixed6480Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Sint3281Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sint3281Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Sint6482Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sint6482Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64String83Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64String83Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Uint3284Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Uint3284Entry)
    - [Proto3MessageLiteWithMaps.FieldMapInt64Uint6485Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Uint6485Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Bool86Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Bool86Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Bytes87Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Bytes87Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Double88Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Double88Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Enum89Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Enum89Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Fixed3290Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Fixed3290Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Fixed6491Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Fixed6491Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Float92Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Float92Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Int3293Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Int3293Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Int6494Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Int6494Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Message95Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Message95Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Sfixed3296Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sfixed3296Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Sfixed6497Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sfixed6497Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Sint3298Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sint3298Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Sint6499Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sint6499Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32String100Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32String100Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Uint32101Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Uint32101Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed32Uint64102Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Uint64102Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Bool103Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Bool103Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Bytes104Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Bytes104Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Double105Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Double105Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Enum106Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Enum106Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Fixed32107Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Fixed32107Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Fixed64108Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Fixed64108Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Float109Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Float109Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Int32110Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Int32110Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Int64111Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Int64111Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Message112Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Message112Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Sfixed32113Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sfixed32113Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Sfixed64114Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sfixed64114Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Sint32115Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sint32115Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Sint64116Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sint64116Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64String117Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64String117Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Uint32118Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Uint32118Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSfixed64Uint64119Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Uint64119Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Bool120Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Bool120Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Bytes121Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Bytes121Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Double122Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Double122Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Enum123Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Enum123Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Fixed32124Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Fixed32124Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Fixed64125Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Fixed64125Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Float126Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Float126Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Int32127Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Int32127Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Int64128Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Int64128Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Message129Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Message129Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Sfixed32130Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sfixed32130Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Sfixed64131Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sfixed64131Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Sint32132Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sint32132Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Sint64133Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sint64133Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32String134Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32String134Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Uint32135Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Uint32135Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint32Uint64136Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Uint64136Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Bool137Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Bool137Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Bytes138Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Bytes138Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Double139Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Double139Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Enum140Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Enum140Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Fixed32141Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Fixed32141Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Fixed64142Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Fixed64142Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Float143Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Float143Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Int32144Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Int32144Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Int64145Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Int64145Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Message146Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Message146Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Sfixed32147Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sfixed32147Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Sfixed64148Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sfixed64148Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Sint32149Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sint32149Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Sint64150Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sint64150Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64String151Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64String151Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Uint32152Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Uint32152Entry)
    - [Proto3MessageLiteWithMaps.FieldMapSint64Uint64153Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Uint64153Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringBool154Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringBool154Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringBytes155Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringBytes155Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringDouble156Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringDouble156Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringEnum157Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringEnum157Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringFixed32158Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFixed32158Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringFixed64159Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFixed64159Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringFloat160Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFloat160Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringInt32161Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringInt32161Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringInt64162Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringInt64162Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringMessage163Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringMessage163Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringSfixed32164Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSfixed32164Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringSfixed64165Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSfixed64165Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringSint32166Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSint32166Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringSint64167Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSint64167Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringString168Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringString168Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringUint32169Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringUint32169Entry)
    - [Proto3MessageLiteWithMaps.FieldMapStringUint64170Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringUint64170Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Bool171Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Bool171Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Bytes172Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Bytes172Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Double173Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Double173Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Enum174Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Enum174Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Fixed32175Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Fixed32175Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Fixed64176Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Fixed64176Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Float177Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Float177Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Int32178Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Int32178Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Int64179Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Int64179Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Message180Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Message180Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Sfixed32181Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sfixed32181Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Sfixed64182Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sfixed64182Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Sint32183Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sint32183Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Sint64184Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sint64184Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32String185Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32String185Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Uint32186Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Uint32186Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint32Uint64187Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Uint64187Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Bool188Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Bool188Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Bytes189Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Bytes189Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Double190Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Double190Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Enum191Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Enum191Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Fixed32192Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Fixed32192Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Fixed64193Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Fixed64193Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Float194Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Float194Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Int32195Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Int32195Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Int64196Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Int64196Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Message197Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Message197Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Sfixed32198Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sfixed32198Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Sfixed64199Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sfixed64199Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Sint32200Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sint32200Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Sint64201Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sint64201Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64String202Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64String202Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Uint32203Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Uint32203Entry)
    - [Proto3MessageLiteWithMaps.FieldMapUint64Uint64204Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Uint64204Entry)
  
    - [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum)
  
- [Scalar Value Types](#scalar-value-types)



<a name="java_core_src_test_proto_com_google_protobuf_proto3_message_lite-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## java/core/src/test/proto/com/google/protobuf/proto3_message_lite.proto



<a name="protobuf-experimental-Proto3EmptyLite"></a>

### Proto3EmptyLite







<a name="protobuf-experimental-Proto3MessageLite"></a>

### Proto3MessageLite



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_double_1 | [double](#double) |  |  |
| field_float_2 | [float](#float) |  |  |
| field_int64_3 | [int64](#int64) |  |  |
| field_uint64_4 | [uint64](#uint64) |  |  |
| field_int32_5 | [int32](#int32) |  |  |
| field_fixed64_6 | [fixed64](#fixed64) |  |  |
| field_fixed32_7 | [fixed32](#fixed32) |  |  |
| field_bool_8 | [bool](#bool) |  |  |
| field_string_9 | [string](#string) |  |  |
| field_message_10 | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |
| field_bytes_11 | [bytes](#bytes) |  |  |
| field_uint32_12 | [uint32](#uint32) |  |  |
| field_enum_13 | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |
| field_sfixed32_14 | [sfixed32](#sfixed32) |  |  |
| field_sfixed64_15 | [sfixed64](#sfixed64) |  |  |
| field_sint32_16 | [sint32](#sint32) |  |  |
| field_sint64_17 | [sint64](#sint64) |  |  |
| field_double_list_18 | [double](#double) | repeated |  |
| field_float_list_19 | [float](#float) | repeated |  |
| field_int64_list_20 | [int64](#int64) | repeated |  |
| field_uint64_list_21 | [uint64](#uint64) | repeated |  |
| field_int32_list_22 | [int32](#int32) | repeated |  |
| field_fixed64_list_23 | [fixed64](#fixed64) | repeated |  |
| field_fixed32_list_24 | [fixed32](#fixed32) | repeated |  |
| field_bool_list_25 | [bool](#bool) | repeated |  |
| field_string_list_26 | [string](#string) | repeated |  |
| field_message_list_27 | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) | repeated |  |
| field_bytes_list_28 | [bytes](#bytes) | repeated |  |
| field_uint32_list_29 | [uint32](#uint32) | repeated |  |
| field_enum_list_30 | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) | repeated |  |
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
| field_enum_list_packed_44 | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) | repeated |  |
| field_sfixed32_list_packed_45 | [sfixed32](#sfixed32) | repeated |  |
| field_sfixed64_list_packed_46 | [sfixed64](#sfixed64) | repeated |  |
| field_sint32_list_packed_47 | [sint32](#sint32) | repeated |  |
| field_sint64_list_packed_48 | [sint64](#sint64) | repeated |  |
| field_double_53 | [double](#double) |  |  |
| field_float_54 | [float](#float) |  |  |
| field_int64_55 | [int64](#int64) |  |  |
| field_uint64_56 | [uint64](#uint64) |  |  |
| field_int32_57 | [int32](#int32) |  |  |
| field_fixed64_58 | [fixed64](#fixed64) |  |  |
| field_fixed32_59 | [fixed32](#fixed32) |  |  |
| field_bool_60 | [bool](#bool) |  |  |
| field_string_61 | [string](#string) |  |  |
| field_message_62 | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |
| field_bytes_63 | [bytes](#bytes) |  |  |
| field_uint32_64 | [uint32](#uint32) |  |  |
| field_sfixed32_65 | [sfixed32](#sfixed32) |  |  |
| field_sfixed64_66 | [sfixed64](#sfixed64) |  |  |
| field_sint32_67 | [sint32](#sint32) |  |  |
| field_sint64_68 | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps"></a>

### Proto3MessageLiteWithMaps



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field_map_bool_bool_1 | [Proto3MessageLiteWithMaps.FieldMapBoolBool1Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolBool1Entry) | repeated |  |
| field_map_bool_bytes_2 | [Proto3MessageLiteWithMaps.FieldMapBoolBytes2Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolBytes2Entry) | repeated |  |
| field_map_bool_double_3 | [Proto3MessageLiteWithMaps.FieldMapBoolDouble3Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolDouble3Entry) | repeated |  |
| field_map_bool_enum_4 | [Proto3MessageLiteWithMaps.FieldMapBoolEnum4Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolEnum4Entry) | repeated |  |
| field_map_bool_fixed32_5 | [Proto3MessageLiteWithMaps.FieldMapBoolFixed325Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFixed325Entry) | repeated |  |
| field_map_bool_fixed64_6 | [Proto3MessageLiteWithMaps.FieldMapBoolFixed646Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFixed646Entry) | repeated |  |
| field_map_bool_float_7 | [Proto3MessageLiteWithMaps.FieldMapBoolFloat7Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFloat7Entry) | repeated |  |
| field_map_bool_int32_8 | [Proto3MessageLiteWithMaps.FieldMapBoolInt328Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolInt328Entry) | repeated |  |
| field_map_bool_int64_9 | [Proto3MessageLiteWithMaps.FieldMapBoolInt649Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolInt649Entry) | repeated |  |
| field_map_bool_message_10 | [Proto3MessageLiteWithMaps.FieldMapBoolMessage10Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolMessage10Entry) | repeated |  |
| field_map_bool_sfixed32_11 | [Proto3MessageLiteWithMaps.FieldMapBoolSfixed3211Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSfixed3211Entry) | repeated |  |
| field_map_bool_sfixed64_12 | [Proto3MessageLiteWithMaps.FieldMapBoolSfixed6412Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSfixed6412Entry) | repeated |  |
| field_map_bool_sint32_13 | [Proto3MessageLiteWithMaps.FieldMapBoolSint3213Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSint3213Entry) | repeated |  |
| field_map_bool_sint64_14 | [Proto3MessageLiteWithMaps.FieldMapBoolSint6414Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSint6414Entry) | repeated |  |
| field_map_bool_string_15 | [Proto3MessageLiteWithMaps.FieldMapBoolString15Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolString15Entry) | repeated |  |
| field_map_bool_uint32_16 | [Proto3MessageLiteWithMaps.FieldMapBoolUint3216Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolUint3216Entry) | repeated |  |
| field_map_bool_uint64_17 | [Proto3MessageLiteWithMaps.FieldMapBoolUint6417Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolUint6417Entry) | repeated |  |
| field_map_fixed32_bool_18 | [Proto3MessageLiteWithMaps.FieldMapFixed32Bool18Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Bool18Entry) | repeated |  |
| field_map_fixed32_bytes_19 | [Proto3MessageLiteWithMaps.FieldMapFixed32Bytes19Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Bytes19Entry) | repeated |  |
| field_map_fixed32_double_20 | [Proto3MessageLiteWithMaps.FieldMapFixed32Double20Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Double20Entry) | repeated |  |
| field_map_fixed32_enum_21 | [Proto3MessageLiteWithMaps.FieldMapFixed32Enum21Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Enum21Entry) | repeated |  |
| field_map_fixed32_fixed32_22 | [Proto3MessageLiteWithMaps.FieldMapFixed32Fixed3222Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Fixed3222Entry) | repeated |  |
| field_map_fixed32_fixed64_23 | [Proto3MessageLiteWithMaps.FieldMapFixed32Fixed6423Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Fixed6423Entry) | repeated |  |
| field_map_fixed32_float_24 | [Proto3MessageLiteWithMaps.FieldMapFixed32Float24Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Float24Entry) | repeated |  |
| field_map_fixed32_int32_25 | [Proto3MessageLiteWithMaps.FieldMapFixed32Int3225Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Int3225Entry) | repeated |  |
| field_map_fixed32_int64_26 | [Proto3MessageLiteWithMaps.FieldMapFixed32Int6426Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Int6426Entry) | repeated |  |
| field_map_fixed32_message_27 | [Proto3MessageLiteWithMaps.FieldMapFixed32Message27Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Message27Entry) | repeated |  |
| field_map_fixed32_sfixed32_28 | [Proto3MessageLiteWithMaps.FieldMapFixed32Sfixed3228Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sfixed3228Entry) | repeated |  |
| field_map_fixed32_sfixed64_29 | [Proto3MessageLiteWithMaps.FieldMapFixed32Sfixed6429Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sfixed6429Entry) | repeated |  |
| field_map_fixed32_sint32_30 | [Proto3MessageLiteWithMaps.FieldMapFixed32Sint3230Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sint3230Entry) | repeated |  |
| field_map_fixed32_sint64_31 | [Proto3MessageLiteWithMaps.FieldMapFixed32Sint6431Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sint6431Entry) | repeated |  |
| field_map_fixed32_string_32 | [Proto3MessageLiteWithMaps.FieldMapFixed32String32Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32String32Entry) | repeated |  |
| field_map_fixed32_uint32_33 | [Proto3MessageLiteWithMaps.FieldMapFixed32Uint3233Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Uint3233Entry) | repeated |  |
| field_map_fixed32_uint64_34 | [Proto3MessageLiteWithMaps.FieldMapFixed32Uint6434Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Uint6434Entry) | repeated |  |
| field_map_fixed64_bool_35 | [Proto3MessageLiteWithMaps.FieldMapFixed64Bool35Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Bool35Entry) | repeated |  |
| field_map_fixed64_bytes_36 | [Proto3MessageLiteWithMaps.FieldMapFixed64Bytes36Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Bytes36Entry) | repeated |  |
| field_map_fixed64_double_37 | [Proto3MessageLiteWithMaps.FieldMapFixed64Double37Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Double37Entry) | repeated |  |
| field_map_fixed64_enum_38 | [Proto3MessageLiteWithMaps.FieldMapFixed64Enum38Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Enum38Entry) | repeated |  |
| field_map_fixed64_fixed32_39 | [Proto3MessageLiteWithMaps.FieldMapFixed64Fixed3239Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Fixed3239Entry) | repeated |  |
| field_map_fixed64_fixed64_40 | [Proto3MessageLiteWithMaps.FieldMapFixed64Fixed6440Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Fixed6440Entry) | repeated |  |
| field_map_fixed64_float_41 | [Proto3MessageLiteWithMaps.FieldMapFixed64Float41Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Float41Entry) | repeated |  |
| field_map_fixed64_int32_42 | [Proto3MessageLiteWithMaps.FieldMapFixed64Int3242Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Int3242Entry) | repeated |  |
| field_map_fixed64_int64_43 | [Proto3MessageLiteWithMaps.FieldMapFixed64Int6443Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Int6443Entry) | repeated |  |
| field_map_fixed64_message_44 | [Proto3MessageLiteWithMaps.FieldMapFixed64Message44Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Message44Entry) | repeated |  |
| field_map_fixed64_sfixed32_45 | [Proto3MessageLiteWithMaps.FieldMapFixed64Sfixed3245Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sfixed3245Entry) | repeated |  |
| field_map_fixed64_sfixed64_46 | [Proto3MessageLiteWithMaps.FieldMapFixed64Sfixed6446Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sfixed6446Entry) | repeated |  |
| field_map_fixed64_sint32_47 | [Proto3MessageLiteWithMaps.FieldMapFixed64Sint3247Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sint3247Entry) | repeated |  |
| field_map_fixed64_sint64_48 | [Proto3MessageLiteWithMaps.FieldMapFixed64Sint6448Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sint6448Entry) | repeated |  |
| field_map_fixed64_string_49 | [Proto3MessageLiteWithMaps.FieldMapFixed64String49Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64String49Entry) | repeated |  |
| field_map_fixed64_uint32_50 | [Proto3MessageLiteWithMaps.FieldMapFixed64Uint3250Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Uint3250Entry) | repeated |  |
| field_map_fixed64_uint64_51 | [Proto3MessageLiteWithMaps.FieldMapFixed64Uint6451Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Uint6451Entry) | repeated |  |
| field_map_int32_bool_52 | [Proto3MessageLiteWithMaps.FieldMapInt32Bool52Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Bool52Entry) | repeated |  |
| field_map_int32_bytes_53 | [Proto3MessageLiteWithMaps.FieldMapInt32Bytes53Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Bytes53Entry) | repeated |  |
| field_map_int32_double_54 | [Proto3MessageLiteWithMaps.FieldMapInt32Double54Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Double54Entry) | repeated |  |
| field_map_int32_enum_55 | [Proto3MessageLiteWithMaps.FieldMapInt32Enum55Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Enum55Entry) | repeated |  |
| field_map_int32_fixed32_56 | [Proto3MessageLiteWithMaps.FieldMapInt32Fixed3256Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Fixed3256Entry) | repeated |  |
| field_map_int32_fixed64_57 | [Proto3MessageLiteWithMaps.FieldMapInt32Fixed6457Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Fixed6457Entry) | repeated |  |
| field_map_int32_float_58 | [Proto3MessageLiteWithMaps.FieldMapInt32Float58Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Float58Entry) | repeated |  |
| field_map_int32_int32_59 | [Proto3MessageLiteWithMaps.FieldMapInt32Int3259Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Int3259Entry) | repeated |  |
| field_map_int32_int64_60 | [Proto3MessageLiteWithMaps.FieldMapInt32Int6460Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Int6460Entry) | repeated |  |
| field_map_int32_message_61 | [Proto3MessageLiteWithMaps.FieldMapInt32Message61Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Message61Entry) | repeated |  |
| field_map_int32_sfixed32_62 | [Proto3MessageLiteWithMaps.FieldMapInt32Sfixed3262Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sfixed3262Entry) | repeated |  |
| field_map_int32_sfixed64_63 | [Proto3MessageLiteWithMaps.FieldMapInt32Sfixed6463Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sfixed6463Entry) | repeated |  |
| field_map_int32_sint32_64 | [Proto3MessageLiteWithMaps.FieldMapInt32Sint3264Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sint3264Entry) | repeated |  |
| field_map_int32_sint64_65 | [Proto3MessageLiteWithMaps.FieldMapInt32Sint6465Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sint6465Entry) | repeated |  |
| field_map_int32_string_66 | [Proto3MessageLiteWithMaps.FieldMapInt32String66Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32String66Entry) | repeated |  |
| field_map_int32_uint32_67 | [Proto3MessageLiteWithMaps.FieldMapInt32Uint3267Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Uint3267Entry) | repeated |  |
| field_map_int32_uint64_68 | [Proto3MessageLiteWithMaps.FieldMapInt32Uint6468Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Uint6468Entry) | repeated |  |
| field_map_int64_bool_69 | [Proto3MessageLiteWithMaps.FieldMapInt64Bool69Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Bool69Entry) | repeated |  |
| field_map_int64_bytes_70 | [Proto3MessageLiteWithMaps.FieldMapInt64Bytes70Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Bytes70Entry) | repeated |  |
| field_map_int64_double_71 | [Proto3MessageLiteWithMaps.FieldMapInt64Double71Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Double71Entry) | repeated |  |
| field_map_int64_enum_72 | [Proto3MessageLiteWithMaps.FieldMapInt64Enum72Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Enum72Entry) | repeated |  |
| field_map_int64_fixed32_73 | [Proto3MessageLiteWithMaps.FieldMapInt64Fixed3273Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Fixed3273Entry) | repeated |  |
| field_map_int64_fixed64_74 | [Proto3MessageLiteWithMaps.FieldMapInt64Fixed6474Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Fixed6474Entry) | repeated |  |
| field_map_int64_float_75 | [Proto3MessageLiteWithMaps.FieldMapInt64Float75Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Float75Entry) | repeated |  |
| field_map_int64_int32_76 | [Proto3MessageLiteWithMaps.FieldMapInt64Int3276Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Int3276Entry) | repeated |  |
| field_map_int64_int64_77 | [Proto3MessageLiteWithMaps.FieldMapInt64Int6477Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Int6477Entry) | repeated |  |
| field_map_int64_message_78 | [Proto3MessageLiteWithMaps.FieldMapInt64Message78Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Message78Entry) | repeated |  |
| field_map_int64_sfixed32_79 | [Proto3MessageLiteWithMaps.FieldMapInt64Sfixed3279Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sfixed3279Entry) | repeated |  |
| field_map_int64_sfixed64_80 | [Proto3MessageLiteWithMaps.FieldMapInt64Sfixed6480Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sfixed6480Entry) | repeated |  |
| field_map_int64_sint32_81 | [Proto3MessageLiteWithMaps.FieldMapInt64Sint3281Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sint3281Entry) | repeated |  |
| field_map_int64_sint64_82 | [Proto3MessageLiteWithMaps.FieldMapInt64Sint6482Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sint6482Entry) | repeated |  |
| field_map_int64_string_83 | [Proto3MessageLiteWithMaps.FieldMapInt64String83Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64String83Entry) | repeated |  |
| field_map_int64_uint32_84 | [Proto3MessageLiteWithMaps.FieldMapInt64Uint3284Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Uint3284Entry) | repeated |  |
| field_map_int64_uint64_85 | [Proto3MessageLiteWithMaps.FieldMapInt64Uint6485Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Uint6485Entry) | repeated |  |
| field_map_sfixed32_bool_86 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Bool86Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Bool86Entry) | repeated |  |
| field_map_sfixed32_bytes_87 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Bytes87Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Bytes87Entry) | repeated |  |
| field_map_sfixed32_double_88 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Double88Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Double88Entry) | repeated |  |
| field_map_sfixed32_enum_89 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Enum89Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Enum89Entry) | repeated |  |
| field_map_sfixed32_fixed32_90 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Fixed3290Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Fixed3290Entry) | repeated |  |
| field_map_sfixed32_fixed64_91 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Fixed6491Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Fixed6491Entry) | repeated |  |
| field_map_sfixed32_float_92 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Float92Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Float92Entry) | repeated |  |
| field_map_sfixed32_int32_93 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Int3293Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Int3293Entry) | repeated |  |
| field_map_sfixed32_int64_94 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Int6494Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Int6494Entry) | repeated |  |
| field_map_sfixed32_message_95 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Message95Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Message95Entry) | repeated |  |
| field_map_sfixed32_sfixed32_96 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Sfixed3296Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sfixed3296Entry) | repeated |  |
| field_map_sfixed32_sfixed64_97 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Sfixed6497Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sfixed6497Entry) | repeated |  |
| field_map_sfixed32_sint32_98 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Sint3298Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sint3298Entry) | repeated |  |
| field_map_sfixed32_sint64_99 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Sint6499Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sint6499Entry) | repeated |  |
| field_map_sfixed32_string_100 | [Proto3MessageLiteWithMaps.FieldMapSfixed32String100Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32String100Entry) | repeated |  |
| field_map_sfixed32_uint32_101 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Uint32101Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Uint32101Entry) | repeated |  |
| field_map_sfixed32_uint64_102 | [Proto3MessageLiteWithMaps.FieldMapSfixed32Uint64102Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Uint64102Entry) | repeated |  |
| field_map_sfixed64_bool_103 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Bool103Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Bool103Entry) | repeated |  |
| field_map_sfixed64_bytes_104 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Bytes104Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Bytes104Entry) | repeated |  |
| field_map_sfixed64_double_105 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Double105Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Double105Entry) | repeated |  |
| field_map_sfixed64_enum_106 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Enum106Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Enum106Entry) | repeated |  |
| field_map_sfixed64_fixed32_107 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Fixed32107Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Fixed32107Entry) | repeated |  |
| field_map_sfixed64_fixed64_108 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Fixed64108Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Fixed64108Entry) | repeated |  |
| field_map_sfixed64_float_109 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Float109Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Float109Entry) | repeated |  |
| field_map_sfixed64_int32_110 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Int32110Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Int32110Entry) | repeated |  |
| field_map_sfixed64_int64_111 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Int64111Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Int64111Entry) | repeated |  |
| field_map_sfixed64_message_112 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Message112Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Message112Entry) | repeated |  |
| field_map_sfixed64_sfixed32_113 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Sfixed32113Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sfixed32113Entry) | repeated |  |
| field_map_sfixed64_sfixed64_114 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Sfixed64114Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sfixed64114Entry) | repeated |  |
| field_map_sfixed64_sint32_115 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Sint32115Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sint32115Entry) | repeated |  |
| field_map_sfixed64_sint64_116 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Sint64116Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sint64116Entry) | repeated |  |
| field_map_sfixed64_string_117 | [Proto3MessageLiteWithMaps.FieldMapSfixed64String117Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64String117Entry) | repeated |  |
| field_map_sfixed64_uint32_118 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Uint32118Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Uint32118Entry) | repeated |  |
| field_map_sfixed64_uint64_119 | [Proto3MessageLiteWithMaps.FieldMapSfixed64Uint64119Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Uint64119Entry) | repeated |  |
| field_map_sint32_bool_120 | [Proto3MessageLiteWithMaps.FieldMapSint32Bool120Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Bool120Entry) | repeated |  |
| field_map_sint32_bytes_121 | [Proto3MessageLiteWithMaps.FieldMapSint32Bytes121Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Bytes121Entry) | repeated |  |
| field_map_sint32_double_122 | [Proto3MessageLiteWithMaps.FieldMapSint32Double122Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Double122Entry) | repeated |  |
| field_map_sint32_enum_123 | [Proto3MessageLiteWithMaps.FieldMapSint32Enum123Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Enum123Entry) | repeated |  |
| field_map_sint32_fixed32_124 | [Proto3MessageLiteWithMaps.FieldMapSint32Fixed32124Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Fixed32124Entry) | repeated |  |
| field_map_sint32_fixed64_125 | [Proto3MessageLiteWithMaps.FieldMapSint32Fixed64125Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Fixed64125Entry) | repeated |  |
| field_map_sint32_float_126 | [Proto3MessageLiteWithMaps.FieldMapSint32Float126Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Float126Entry) | repeated |  |
| field_map_sint32_int32_127 | [Proto3MessageLiteWithMaps.FieldMapSint32Int32127Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Int32127Entry) | repeated |  |
| field_map_sint32_int64_128 | [Proto3MessageLiteWithMaps.FieldMapSint32Int64128Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Int64128Entry) | repeated |  |
| field_map_sint32_message_129 | [Proto3MessageLiteWithMaps.FieldMapSint32Message129Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Message129Entry) | repeated |  |
| field_map_sint32_sfixed32_130 | [Proto3MessageLiteWithMaps.FieldMapSint32Sfixed32130Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sfixed32130Entry) | repeated |  |
| field_map_sint32_sfixed64_131 | [Proto3MessageLiteWithMaps.FieldMapSint32Sfixed64131Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sfixed64131Entry) | repeated |  |
| field_map_sint32_sint32_132 | [Proto3MessageLiteWithMaps.FieldMapSint32Sint32132Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sint32132Entry) | repeated |  |
| field_map_sint32_sint64_133 | [Proto3MessageLiteWithMaps.FieldMapSint32Sint64133Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sint64133Entry) | repeated |  |
| field_map_sint32_string_134 | [Proto3MessageLiteWithMaps.FieldMapSint32String134Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32String134Entry) | repeated |  |
| field_map_sint32_uint32_135 | [Proto3MessageLiteWithMaps.FieldMapSint32Uint32135Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Uint32135Entry) | repeated |  |
| field_map_sint32_uint64_136 | [Proto3MessageLiteWithMaps.FieldMapSint32Uint64136Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Uint64136Entry) | repeated |  |
| field_map_sint64_bool_137 | [Proto3MessageLiteWithMaps.FieldMapSint64Bool137Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Bool137Entry) | repeated |  |
| field_map_sint64_bytes_138 | [Proto3MessageLiteWithMaps.FieldMapSint64Bytes138Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Bytes138Entry) | repeated |  |
| field_map_sint64_double_139 | [Proto3MessageLiteWithMaps.FieldMapSint64Double139Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Double139Entry) | repeated |  |
| field_map_sint64_enum_140 | [Proto3MessageLiteWithMaps.FieldMapSint64Enum140Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Enum140Entry) | repeated |  |
| field_map_sint64_fixed32_141 | [Proto3MessageLiteWithMaps.FieldMapSint64Fixed32141Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Fixed32141Entry) | repeated |  |
| field_map_sint64_fixed64_142 | [Proto3MessageLiteWithMaps.FieldMapSint64Fixed64142Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Fixed64142Entry) | repeated |  |
| field_map_sint64_float_143 | [Proto3MessageLiteWithMaps.FieldMapSint64Float143Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Float143Entry) | repeated |  |
| field_map_sint64_int32_144 | [Proto3MessageLiteWithMaps.FieldMapSint64Int32144Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Int32144Entry) | repeated |  |
| field_map_sint64_int64_145 | [Proto3MessageLiteWithMaps.FieldMapSint64Int64145Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Int64145Entry) | repeated |  |
| field_map_sint64_message_146 | [Proto3MessageLiteWithMaps.FieldMapSint64Message146Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Message146Entry) | repeated |  |
| field_map_sint64_sfixed32_147 | [Proto3MessageLiteWithMaps.FieldMapSint64Sfixed32147Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sfixed32147Entry) | repeated |  |
| field_map_sint64_sfixed64_148 | [Proto3MessageLiteWithMaps.FieldMapSint64Sfixed64148Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sfixed64148Entry) | repeated |  |
| field_map_sint64_sint32_149 | [Proto3MessageLiteWithMaps.FieldMapSint64Sint32149Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sint32149Entry) | repeated |  |
| field_map_sint64_sint64_150 | [Proto3MessageLiteWithMaps.FieldMapSint64Sint64150Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sint64150Entry) | repeated |  |
| field_map_sint64_string_151 | [Proto3MessageLiteWithMaps.FieldMapSint64String151Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64String151Entry) | repeated |  |
| field_map_sint64_uint32_152 | [Proto3MessageLiteWithMaps.FieldMapSint64Uint32152Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Uint32152Entry) | repeated |  |
| field_map_sint64_uint64_153 | [Proto3MessageLiteWithMaps.FieldMapSint64Uint64153Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Uint64153Entry) | repeated |  |
| field_map_string_bool_154 | [Proto3MessageLiteWithMaps.FieldMapStringBool154Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringBool154Entry) | repeated |  |
| field_map_string_bytes_155 | [Proto3MessageLiteWithMaps.FieldMapStringBytes155Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringBytes155Entry) | repeated |  |
| field_map_string_double_156 | [Proto3MessageLiteWithMaps.FieldMapStringDouble156Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringDouble156Entry) | repeated |  |
| field_map_string_enum_157 | [Proto3MessageLiteWithMaps.FieldMapStringEnum157Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringEnum157Entry) | repeated |  |
| field_map_string_fixed32_158 | [Proto3MessageLiteWithMaps.FieldMapStringFixed32158Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFixed32158Entry) | repeated |  |
| field_map_string_fixed64_159 | [Proto3MessageLiteWithMaps.FieldMapStringFixed64159Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFixed64159Entry) | repeated |  |
| field_map_string_float_160 | [Proto3MessageLiteWithMaps.FieldMapStringFloat160Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFloat160Entry) | repeated |  |
| field_map_string_int32_161 | [Proto3MessageLiteWithMaps.FieldMapStringInt32161Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringInt32161Entry) | repeated |  |
| field_map_string_int64_162 | [Proto3MessageLiteWithMaps.FieldMapStringInt64162Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringInt64162Entry) | repeated |  |
| field_map_string_message_163 | [Proto3MessageLiteWithMaps.FieldMapStringMessage163Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringMessage163Entry) | repeated |  |
| field_map_string_sfixed32_164 | [Proto3MessageLiteWithMaps.FieldMapStringSfixed32164Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSfixed32164Entry) | repeated |  |
| field_map_string_sfixed64_165 | [Proto3MessageLiteWithMaps.FieldMapStringSfixed64165Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSfixed64165Entry) | repeated |  |
| field_map_string_sint32_166 | [Proto3MessageLiteWithMaps.FieldMapStringSint32166Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSint32166Entry) | repeated |  |
| field_map_string_sint64_167 | [Proto3MessageLiteWithMaps.FieldMapStringSint64167Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSint64167Entry) | repeated |  |
| field_map_string_string_168 | [Proto3MessageLiteWithMaps.FieldMapStringString168Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringString168Entry) | repeated |  |
| field_map_string_uint32_169 | [Proto3MessageLiteWithMaps.FieldMapStringUint32169Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringUint32169Entry) | repeated |  |
| field_map_string_uint64_170 | [Proto3MessageLiteWithMaps.FieldMapStringUint64170Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringUint64170Entry) | repeated |  |
| field_map_uint32_bool_171 | [Proto3MessageLiteWithMaps.FieldMapUint32Bool171Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Bool171Entry) | repeated |  |
| field_map_uint32_bytes_172 | [Proto3MessageLiteWithMaps.FieldMapUint32Bytes172Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Bytes172Entry) | repeated |  |
| field_map_uint32_double_173 | [Proto3MessageLiteWithMaps.FieldMapUint32Double173Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Double173Entry) | repeated |  |
| field_map_uint32_enum_174 | [Proto3MessageLiteWithMaps.FieldMapUint32Enum174Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Enum174Entry) | repeated |  |
| field_map_uint32_fixed32_175 | [Proto3MessageLiteWithMaps.FieldMapUint32Fixed32175Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Fixed32175Entry) | repeated |  |
| field_map_uint32_fixed64_176 | [Proto3MessageLiteWithMaps.FieldMapUint32Fixed64176Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Fixed64176Entry) | repeated |  |
| field_map_uint32_float_177 | [Proto3MessageLiteWithMaps.FieldMapUint32Float177Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Float177Entry) | repeated |  |
| field_map_uint32_int32_178 | [Proto3MessageLiteWithMaps.FieldMapUint32Int32178Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Int32178Entry) | repeated |  |
| field_map_uint32_int64_179 | [Proto3MessageLiteWithMaps.FieldMapUint32Int64179Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Int64179Entry) | repeated |  |
| field_map_uint32_message_180 | [Proto3MessageLiteWithMaps.FieldMapUint32Message180Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Message180Entry) | repeated |  |
| field_map_uint32_sfixed32_181 | [Proto3MessageLiteWithMaps.FieldMapUint32Sfixed32181Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sfixed32181Entry) | repeated |  |
| field_map_uint32_sfixed64_182 | [Proto3MessageLiteWithMaps.FieldMapUint32Sfixed64182Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sfixed64182Entry) | repeated |  |
| field_map_uint32_sint32_183 | [Proto3MessageLiteWithMaps.FieldMapUint32Sint32183Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sint32183Entry) | repeated |  |
| field_map_uint32_sint64_184 | [Proto3MessageLiteWithMaps.FieldMapUint32Sint64184Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sint64184Entry) | repeated |  |
| field_map_uint32_string_185 | [Proto3MessageLiteWithMaps.FieldMapUint32String185Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32String185Entry) | repeated |  |
| field_map_uint32_uint32_186 | [Proto3MessageLiteWithMaps.FieldMapUint32Uint32186Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Uint32186Entry) | repeated |  |
| field_map_uint32_uint64_187 | [Proto3MessageLiteWithMaps.FieldMapUint32Uint64187Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Uint64187Entry) | repeated |  |
| field_map_uint64_bool_188 | [Proto3MessageLiteWithMaps.FieldMapUint64Bool188Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Bool188Entry) | repeated |  |
| field_map_uint64_bytes_189 | [Proto3MessageLiteWithMaps.FieldMapUint64Bytes189Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Bytes189Entry) | repeated |  |
| field_map_uint64_double_190 | [Proto3MessageLiteWithMaps.FieldMapUint64Double190Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Double190Entry) | repeated |  |
| field_map_uint64_enum_191 | [Proto3MessageLiteWithMaps.FieldMapUint64Enum191Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Enum191Entry) | repeated |  |
| field_map_uint64_fixed32_192 | [Proto3MessageLiteWithMaps.FieldMapUint64Fixed32192Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Fixed32192Entry) | repeated |  |
| field_map_uint64_fixed64_193 | [Proto3MessageLiteWithMaps.FieldMapUint64Fixed64193Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Fixed64193Entry) | repeated |  |
| field_map_uint64_float_194 | [Proto3MessageLiteWithMaps.FieldMapUint64Float194Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Float194Entry) | repeated |  |
| field_map_uint64_int32_195 | [Proto3MessageLiteWithMaps.FieldMapUint64Int32195Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Int32195Entry) | repeated |  |
| field_map_uint64_int64_196 | [Proto3MessageLiteWithMaps.FieldMapUint64Int64196Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Int64196Entry) | repeated |  |
| field_map_uint64_message_197 | [Proto3MessageLiteWithMaps.FieldMapUint64Message197Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Message197Entry) | repeated |  |
| field_map_uint64_sfixed32_198 | [Proto3MessageLiteWithMaps.FieldMapUint64Sfixed32198Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sfixed32198Entry) | repeated |  |
| field_map_uint64_sfixed64_199 | [Proto3MessageLiteWithMaps.FieldMapUint64Sfixed64199Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sfixed64199Entry) | repeated |  |
| field_map_uint64_sint32_200 | [Proto3MessageLiteWithMaps.FieldMapUint64Sint32200Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sint32200Entry) | repeated |  |
| field_map_uint64_sint64_201 | [Proto3MessageLiteWithMaps.FieldMapUint64Sint64201Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sint64201Entry) | repeated |  |
| field_map_uint64_string_202 | [Proto3MessageLiteWithMaps.FieldMapUint64String202Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64String202Entry) | repeated |  |
| field_map_uint64_uint32_203 | [Proto3MessageLiteWithMaps.FieldMapUint64Uint32203Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Uint32203Entry) | repeated |  |
| field_map_uint64_uint64_204 | [Proto3MessageLiteWithMaps.FieldMapUint64Uint64204Entry](#protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Uint64204Entry) | repeated |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolBool1Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolBool1Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolBytes2Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolBytes2Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolDouble3Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolDouble3Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolEnum4Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolEnum4Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFixed325Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolFixed325Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFixed646Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolFixed646Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolFloat7Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolFloat7Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolInt328Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolInt328Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolInt649Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolInt649Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolMessage10Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolMessage10Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSfixed3211Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolSfixed3211Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSfixed6412Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolSfixed6412Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSint3213Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolSint3213Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolSint6414Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolSint6414Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolString15Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolString15Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolUint3216Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolUint3216Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapBoolUint6417Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapBoolUint6417Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [bool](#bool) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Bool18Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Bool18Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Bytes19Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Bytes19Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Double20Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Double20Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Enum21Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Enum21Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Fixed3222Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Fixed3222Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Fixed6423Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Fixed6423Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Float24Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Float24Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Int3225Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Int3225Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Int6426Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Int6426Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Message27Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Message27Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sfixed3228Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Sfixed3228Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sfixed6429Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Sfixed6429Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sint3230Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Sint3230Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Sint6431Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Sint6431Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32String32Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32String32Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Uint3233Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Uint3233Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed32Uint6434Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed32Uint6434Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed32](#fixed32) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Bool35Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Bool35Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Bytes36Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Bytes36Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Double37Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Double37Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Enum38Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Enum38Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Fixed3239Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Fixed3239Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Fixed6440Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Fixed6440Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Float41Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Float41Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Int3242Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Int3242Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Int6443Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Int6443Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Message44Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Message44Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sfixed3245Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Sfixed3245Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sfixed6446Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Sfixed6446Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sint3247Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Sint3247Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Sint6448Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Sint6448Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64String49Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64String49Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Uint3250Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Uint3250Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapFixed64Uint6451Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapFixed64Uint6451Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [fixed64](#fixed64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Bool52Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Bool52Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Bytes53Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Bytes53Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Double54Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Double54Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Enum55Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Enum55Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Fixed3256Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Fixed3256Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Fixed6457Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Fixed6457Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Float58Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Float58Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Int3259Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Int3259Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Int6460Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Int6460Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Message61Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Message61Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sfixed3262Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Sfixed3262Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sfixed6463Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Sfixed6463Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sint3264Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Sint3264Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Sint6465Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Sint6465Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32String66Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32String66Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Uint3267Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Uint3267Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt32Uint6468Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt32Uint6468Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Bool69Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Bool69Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Bytes70Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Bytes70Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Double71Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Double71Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Enum72Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Enum72Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Fixed3273Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Fixed3273Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Fixed6474Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Fixed6474Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Float75Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Float75Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Int3276Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Int3276Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Int6477Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Int6477Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Message78Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Message78Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sfixed3279Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Sfixed3279Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sfixed6480Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Sfixed6480Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sint3281Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Sint3281Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Sint6482Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Sint6482Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64String83Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64String83Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Uint3284Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Uint3284Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapInt64Uint6485Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapInt64Uint6485Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int64](#int64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Bool86Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Bool86Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Bytes87Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Bytes87Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Double88Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Double88Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Enum89Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Enum89Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Fixed3290Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Fixed3290Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Fixed6491Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Fixed6491Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Float92Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Float92Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Int3293Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Int3293Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Int6494Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Int6494Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Message95Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Message95Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sfixed3296Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Sfixed3296Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sfixed6497Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Sfixed6497Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sint3298Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Sint3298Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Sint6499Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Sint6499Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32String100Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32String100Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Uint32101Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Uint32101Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed32Uint64102Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed32Uint64102Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed32](#sfixed32) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Bool103Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Bool103Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Bytes104Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Bytes104Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Double105Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Double105Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Enum106Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Enum106Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Fixed32107Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Fixed32107Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Fixed64108Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Fixed64108Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Float109Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Float109Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Int32110Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Int32110Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Int64111Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Int64111Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Message112Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Message112Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sfixed32113Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Sfixed32113Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sfixed64114Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Sfixed64114Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sint32115Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Sint32115Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Sint64116Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Sint64116Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64String117Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64String117Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Uint32118Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Uint32118Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSfixed64Uint64119Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSfixed64Uint64119Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sfixed64](#sfixed64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Bool120Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Bool120Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Bytes121Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Bytes121Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Double122Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Double122Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Enum123Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Enum123Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Fixed32124Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Fixed32124Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Fixed64125Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Fixed64125Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Float126Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Float126Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Int32127Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Int32127Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Int64128Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Int64128Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Message129Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Message129Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sfixed32130Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Sfixed32130Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sfixed64131Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Sfixed64131Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sint32132Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Sint32132Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Sint64133Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Sint64133Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32String134Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32String134Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Uint32135Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Uint32135Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint32Uint64136Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint32Uint64136Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint32](#sint32) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Bool137Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Bool137Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Bytes138Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Bytes138Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Double139Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Double139Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Enum140Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Enum140Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Fixed32141Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Fixed32141Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Fixed64142Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Fixed64142Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Float143Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Float143Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Int32144Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Int32144Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Int64145Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Int64145Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Message146Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Message146Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sfixed32147Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Sfixed32147Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sfixed64148Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Sfixed64148Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sint32149Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Sint32149Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Sint64150Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Sint64150Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64String151Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64String151Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Uint32152Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Uint32152Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapSint64Uint64153Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapSint64Uint64153Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [sint64](#sint64) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringBool154Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringBool154Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringBytes155Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringBytes155Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringDouble156Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringDouble156Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringEnum157Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringEnum157Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFixed32158Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringFixed32158Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFixed64159Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringFixed64159Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringFloat160Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringFloat160Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringInt32161Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringInt32161Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringInt64162Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringInt64162Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringMessage163Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringMessage163Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSfixed32164Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringSfixed32164Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSfixed64165Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringSfixed64165Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSint32166Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringSint32166Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringSint64167Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringSint64167Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringString168Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringString168Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringUint32169Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringUint32169Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapStringUint64170Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapStringUint64170Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Bool171Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Bool171Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Bytes172Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Bytes172Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Double173Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Double173Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Enum174Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Enum174Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Fixed32175Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Fixed32175Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Fixed64176Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Fixed64176Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Float177Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Float177Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Int32178Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Int32178Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Int64179Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Int64179Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Message180Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Message180Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sfixed32181Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Sfixed32181Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sfixed64182Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Sfixed64182Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sint32183Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Sint32183Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Sint64184Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Sint64184Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32String185Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32String185Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Uint32186Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Uint32186Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint32Uint64187Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint32Uint64187Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [uint64](#uint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Bool188Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Bool188Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [bool](#bool) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Bytes189Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Bytes189Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [bytes](#bytes) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Double190Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Double190Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [double](#double) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Enum191Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Enum191Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [Proto3MessageLite.TestEnum](#protobuf-experimental-Proto3MessageLite-TestEnum) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Fixed32192Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Fixed32192Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [fixed32](#fixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Fixed64193Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Fixed64193Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [fixed64](#fixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Float194Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Float194Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [float](#float) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Int32195Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Int32195Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [int32](#int32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Int64196Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Int64196Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [int64](#int64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Message197Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Message197Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [Proto3MessageLite](#protobuf-experimental-Proto3MessageLite) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sfixed32198Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Sfixed32198Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [sfixed32](#sfixed32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sfixed64199Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Sfixed64199Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [sfixed64](#sfixed64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sint32200Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Sint32200Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [sint32](#sint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Sint64201Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Sint64201Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [sint64](#sint64) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64String202Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64String202Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [string](#string) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Uint32203Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Uint32203Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [uint32](#uint32) |  |  |






<a name="protobuf-experimental-Proto3MessageLiteWithMaps-FieldMapUint64Uint64204Entry"></a>

### Proto3MessageLiteWithMaps.FieldMapUint64Uint64204Entry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint64](#uint64) |  |  |
| value | [uint64](#uint64) |  |  |





 


<a name="protobuf-experimental-Proto3MessageLite-TestEnum"></a>

### Proto3MessageLite.TestEnum


| Name | Number | Description |
| ---- | ------ | ----------- |
| ZERO | 0 |  |
| ONE | 1 |  |
| TWO | 2 |  |


 

 

 



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

