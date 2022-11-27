# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [python/google/protobuf/internal/more_messages.proto](#python_google_protobuf_internal_more_messages-proto)
    - [ExtendClass](#google-protobuf-internal-ExtendClass)
    - [LotsNestedMessage](#google-protobuf-internal-LotsNestedMessage)
    - [LotsNestedMessage.B0](#google-protobuf-internal-LotsNestedMessage-B0)
    - [LotsNestedMessage.B1](#google-protobuf-internal-LotsNestedMessage-B1)
    - [LotsNestedMessage.B10](#google-protobuf-internal-LotsNestedMessage-B10)
    - [LotsNestedMessage.B100](#google-protobuf-internal-LotsNestedMessage-B100)
    - [LotsNestedMessage.B101](#google-protobuf-internal-LotsNestedMessage-B101)
    - [LotsNestedMessage.B102](#google-protobuf-internal-LotsNestedMessage-B102)
    - [LotsNestedMessage.B103](#google-protobuf-internal-LotsNestedMessage-B103)
    - [LotsNestedMessage.B104](#google-protobuf-internal-LotsNestedMessage-B104)
    - [LotsNestedMessage.B105](#google-protobuf-internal-LotsNestedMessage-B105)
    - [LotsNestedMessage.B106](#google-protobuf-internal-LotsNestedMessage-B106)
    - [LotsNestedMessage.B107](#google-protobuf-internal-LotsNestedMessage-B107)
    - [LotsNestedMessage.B108](#google-protobuf-internal-LotsNestedMessage-B108)
    - [LotsNestedMessage.B109](#google-protobuf-internal-LotsNestedMessage-B109)
    - [LotsNestedMessage.B11](#google-protobuf-internal-LotsNestedMessage-B11)
    - [LotsNestedMessage.B110](#google-protobuf-internal-LotsNestedMessage-B110)
    - [LotsNestedMessage.B111](#google-protobuf-internal-LotsNestedMessage-B111)
    - [LotsNestedMessage.B112](#google-protobuf-internal-LotsNestedMessage-B112)
    - [LotsNestedMessage.B113](#google-protobuf-internal-LotsNestedMessage-B113)
    - [LotsNestedMessage.B114](#google-protobuf-internal-LotsNestedMessage-B114)
    - [LotsNestedMessage.B115](#google-protobuf-internal-LotsNestedMessage-B115)
    - [LotsNestedMessage.B116](#google-protobuf-internal-LotsNestedMessage-B116)
    - [LotsNestedMessage.B117](#google-protobuf-internal-LotsNestedMessage-B117)
    - [LotsNestedMessage.B118](#google-protobuf-internal-LotsNestedMessage-B118)
    - [LotsNestedMessage.B119](#google-protobuf-internal-LotsNestedMessage-B119)
    - [LotsNestedMessage.B12](#google-protobuf-internal-LotsNestedMessage-B12)
    - [LotsNestedMessage.B120](#google-protobuf-internal-LotsNestedMessage-B120)
    - [LotsNestedMessage.B121](#google-protobuf-internal-LotsNestedMessage-B121)
    - [LotsNestedMessage.B122](#google-protobuf-internal-LotsNestedMessage-B122)
    - [LotsNestedMessage.B123](#google-protobuf-internal-LotsNestedMessage-B123)
    - [LotsNestedMessage.B124](#google-protobuf-internal-LotsNestedMessage-B124)
    - [LotsNestedMessage.B125](#google-protobuf-internal-LotsNestedMessage-B125)
    - [LotsNestedMessage.B126](#google-protobuf-internal-LotsNestedMessage-B126)
    - [LotsNestedMessage.B127](#google-protobuf-internal-LotsNestedMessage-B127)
    - [LotsNestedMessage.B128](#google-protobuf-internal-LotsNestedMessage-B128)
    - [LotsNestedMessage.B129](#google-protobuf-internal-LotsNestedMessage-B129)
    - [LotsNestedMessage.B13](#google-protobuf-internal-LotsNestedMessage-B13)
    - [LotsNestedMessage.B130](#google-protobuf-internal-LotsNestedMessage-B130)
    - [LotsNestedMessage.B131](#google-protobuf-internal-LotsNestedMessage-B131)
    - [LotsNestedMessage.B132](#google-protobuf-internal-LotsNestedMessage-B132)
    - [LotsNestedMessage.B133](#google-protobuf-internal-LotsNestedMessage-B133)
    - [LotsNestedMessage.B134](#google-protobuf-internal-LotsNestedMessage-B134)
    - [LotsNestedMessage.B135](#google-protobuf-internal-LotsNestedMessage-B135)
    - [LotsNestedMessage.B136](#google-protobuf-internal-LotsNestedMessage-B136)
    - [LotsNestedMessage.B137](#google-protobuf-internal-LotsNestedMessage-B137)
    - [LotsNestedMessage.B138](#google-protobuf-internal-LotsNestedMessage-B138)
    - [LotsNestedMessage.B139](#google-protobuf-internal-LotsNestedMessage-B139)
    - [LotsNestedMessage.B14](#google-protobuf-internal-LotsNestedMessage-B14)
    - [LotsNestedMessage.B140](#google-protobuf-internal-LotsNestedMessage-B140)
    - [LotsNestedMessage.B141](#google-protobuf-internal-LotsNestedMessage-B141)
    - [LotsNestedMessage.B142](#google-protobuf-internal-LotsNestedMessage-B142)
    - [LotsNestedMessage.B143](#google-protobuf-internal-LotsNestedMessage-B143)
    - [LotsNestedMessage.B144](#google-protobuf-internal-LotsNestedMessage-B144)
    - [LotsNestedMessage.B145](#google-protobuf-internal-LotsNestedMessage-B145)
    - [LotsNestedMessage.B146](#google-protobuf-internal-LotsNestedMessage-B146)
    - [LotsNestedMessage.B147](#google-protobuf-internal-LotsNestedMessage-B147)
    - [LotsNestedMessage.B148](#google-protobuf-internal-LotsNestedMessage-B148)
    - [LotsNestedMessage.B149](#google-protobuf-internal-LotsNestedMessage-B149)
    - [LotsNestedMessage.B15](#google-protobuf-internal-LotsNestedMessage-B15)
    - [LotsNestedMessage.B150](#google-protobuf-internal-LotsNestedMessage-B150)
    - [LotsNestedMessage.B151](#google-protobuf-internal-LotsNestedMessage-B151)
    - [LotsNestedMessage.B152](#google-protobuf-internal-LotsNestedMessage-B152)
    - [LotsNestedMessage.B153](#google-protobuf-internal-LotsNestedMessage-B153)
    - [LotsNestedMessage.B154](#google-protobuf-internal-LotsNestedMessage-B154)
    - [LotsNestedMessage.B155](#google-protobuf-internal-LotsNestedMessage-B155)
    - [LotsNestedMessage.B156](#google-protobuf-internal-LotsNestedMessage-B156)
    - [LotsNestedMessage.B157](#google-protobuf-internal-LotsNestedMessage-B157)
    - [LotsNestedMessage.B158](#google-protobuf-internal-LotsNestedMessage-B158)
    - [LotsNestedMessage.B159](#google-protobuf-internal-LotsNestedMessage-B159)
    - [LotsNestedMessage.B16](#google-protobuf-internal-LotsNestedMessage-B16)
    - [LotsNestedMessage.B160](#google-protobuf-internal-LotsNestedMessage-B160)
    - [LotsNestedMessage.B161](#google-protobuf-internal-LotsNestedMessage-B161)
    - [LotsNestedMessage.B162](#google-protobuf-internal-LotsNestedMessage-B162)
    - [LotsNestedMessage.B163](#google-protobuf-internal-LotsNestedMessage-B163)
    - [LotsNestedMessage.B164](#google-protobuf-internal-LotsNestedMessage-B164)
    - [LotsNestedMessage.B165](#google-protobuf-internal-LotsNestedMessage-B165)
    - [LotsNestedMessage.B166](#google-protobuf-internal-LotsNestedMessage-B166)
    - [LotsNestedMessage.B167](#google-protobuf-internal-LotsNestedMessage-B167)
    - [LotsNestedMessage.B168](#google-protobuf-internal-LotsNestedMessage-B168)
    - [LotsNestedMessage.B169](#google-protobuf-internal-LotsNestedMessage-B169)
    - [LotsNestedMessage.B17](#google-protobuf-internal-LotsNestedMessage-B17)
    - [LotsNestedMessage.B170](#google-protobuf-internal-LotsNestedMessage-B170)
    - [LotsNestedMessage.B171](#google-protobuf-internal-LotsNestedMessage-B171)
    - [LotsNestedMessage.B172](#google-protobuf-internal-LotsNestedMessage-B172)
    - [LotsNestedMessage.B173](#google-protobuf-internal-LotsNestedMessage-B173)
    - [LotsNestedMessage.B174](#google-protobuf-internal-LotsNestedMessage-B174)
    - [LotsNestedMessage.B175](#google-protobuf-internal-LotsNestedMessage-B175)
    - [LotsNestedMessage.B176](#google-protobuf-internal-LotsNestedMessage-B176)
    - [LotsNestedMessage.B177](#google-protobuf-internal-LotsNestedMessage-B177)
    - [LotsNestedMessage.B178](#google-protobuf-internal-LotsNestedMessage-B178)
    - [LotsNestedMessage.B179](#google-protobuf-internal-LotsNestedMessage-B179)
    - [LotsNestedMessage.B18](#google-protobuf-internal-LotsNestedMessage-B18)
    - [LotsNestedMessage.B180](#google-protobuf-internal-LotsNestedMessage-B180)
    - [LotsNestedMessage.B181](#google-protobuf-internal-LotsNestedMessage-B181)
    - [LotsNestedMessage.B182](#google-protobuf-internal-LotsNestedMessage-B182)
    - [LotsNestedMessage.B183](#google-protobuf-internal-LotsNestedMessage-B183)
    - [LotsNestedMessage.B184](#google-protobuf-internal-LotsNestedMessage-B184)
    - [LotsNestedMessage.B185](#google-protobuf-internal-LotsNestedMessage-B185)
    - [LotsNestedMessage.B186](#google-protobuf-internal-LotsNestedMessage-B186)
    - [LotsNestedMessage.B187](#google-protobuf-internal-LotsNestedMessage-B187)
    - [LotsNestedMessage.B188](#google-protobuf-internal-LotsNestedMessage-B188)
    - [LotsNestedMessage.B189](#google-protobuf-internal-LotsNestedMessage-B189)
    - [LotsNestedMessage.B19](#google-protobuf-internal-LotsNestedMessage-B19)
    - [LotsNestedMessage.B190](#google-protobuf-internal-LotsNestedMessage-B190)
    - [LotsNestedMessage.B191](#google-protobuf-internal-LotsNestedMessage-B191)
    - [LotsNestedMessage.B192](#google-protobuf-internal-LotsNestedMessage-B192)
    - [LotsNestedMessage.B193](#google-protobuf-internal-LotsNestedMessage-B193)
    - [LotsNestedMessage.B194](#google-protobuf-internal-LotsNestedMessage-B194)
    - [LotsNestedMessage.B195](#google-protobuf-internal-LotsNestedMessage-B195)
    - [LotsNestedMessage.B196](#google-protobuf-internal-LotsNestedMessage-B196)
    - [LotsNestedMessage.B197](#google-protobuf-internal-LotsNestedMessage-B197)
    - [LotsNestedMessage.B198](#google-protobuf-internal-LotsNestedMessage-B198)
    - [LotsNestedMessage.B199](#google-protobuf-internal-LotsNestedMessage-B199)
    - [LotsNestedMessage.B2](#google-protobuf-internal-LotsNestedMessage-B2)
    - [LotsNestedMessage.B20](#google-protobuf-internal-LotsNestedMessage-B20)
    - [LotsNestedMessage.B200](#google-protobuf-internal-LotsNestedMessage-B200)
    - [LotsNestedMessage.B201](#google-protobuf-internal-LotsNestedMessage-B201)
    - [LotsNestedMessage.B202](#google-protobuf-internal-LotsNestedMessage-B202)
    - [LotsNestedMessage.B203](#google-protobuf-internal-LotsNestedMessage-B203)
    - [LotsNestedMessage.B204](#google-protobuf-internal-LotsNestedMessage-B204)
    - [LotsNestedMessage.B205](#google-protobuf-internal-LotsNestedMessage-B205)
    - [LotsNestedMessage.B206](#google-protobuf-internal-LotsNestedMessage-B206)
    - [LotsNestedMessage.B207](#google-protobuf-internal-LotsNestedMessage-B207)
    - [LotsNestedMessage.B208](#google-protobuf-internal-LotsNestedMessage-B208)
    - [LotsNestedMessage.B209](#google-protobuf-internal-LotsNestedMessage-B209)
    - [LotsNestedMessage.B21](#google-protobuf-internal-LotsNestedMessage-B21)
    - [LotsNestedMessage.B210](#google-protobuf-internal-LotsNestedMessage-B210)
    - [LotsNestedMessage.B211](#google-protobuf-internal-LotsNestedMessage-B211)
    - [LotsNestedMessage.B212](#google-protobuf-internal-LotsNestedMessage-B212)
    - [LotsNestedMessage.B213](#google-protobuf-internal-LotsNestedMessage-B213)
    - [LotsNestedMessage.B214](#google-protobuf-internal-LotsNestedMessage-B214)
    - [LotsNestedMessage.B215](#google-protobuf-internal-LotsNestedMessage-B215)
    - [LotsNestedMessage.B216](#google-protobuf-internal-LotsNestedMessage-B216)
    - [LotsNestedMessage.B217](#google-protobuf-internal-LotsNestedMessage-B217)
    - [LotsNestedMessage.B218](#google-protobuf-internal-LotsNestedMessage-B218)
    - [LotsNestedMessage.B219](#google-protobuf-internal-LotsNestedMessage-B219)
    - [LotsNestedMessage.B22](#google-protobuf-internal-LotsNestedMessage-B22)
    - [LotsNestedMessage.B220](#google-protobuf-internal-LotsNestedMessage-B220)
    - [LotsNestedMessage.B221](#google-protobuf-internal-LotsNestedMessage-B221)
    - [LotsNestedMessage.B222](#google-protobuf-internal-LotsNestedMessage-B222)
    - [LotsNestedMessage.B223](#google-protobuf-internal-LotsNestedMessage-B223)
    - [LotsNestedMessage.B224](#google-protobuf-internal-LotsNestedMessage-B224)
    - [LotsNestedMessage.B225](#google-protobuf-internal-LotsNestedMessage-B225)
    - [LotsNestedMessage.B226](#google-protobuf-internal-LotsNestedMessage-B226)
    - [LotsNestedMessage.B227](#google-protobuf-internal-LotsNestedMessage-B227)
    - [LotsNestedMessage.B228](#google-protobuf-internal-LotsNestedMessage-B228)
    - [LotsNestedMessage.B229](#google-protobuf-internal-LotsNestedMessage-B229)
    - [LotsNestedMessage.B23](#google-protobuf-internal-LotsNestedMessage-B23)
    - [LotsNestedMessage.B230](#google-protobuf-internal-LotsNestedMessage-B230)
    - [LotsNestedMessage.B231](#google-protobuf-internal-LotsNestedMessage-B231)
    - [LotsNestedMessage.B232](#google-protobuf-internal-LotsNestedMessage-B232)
    - [LotsNestedMessage.B233](#google-protobuf-internal-LotsNestedMessage-B233)
    - [LotsNestedMessage.B234](#google-protobuf-internal-LotsNestedMessage-B234)
    - [LotsNestedMessage.B235](#google-protobuf-internal-LotsNestedMessage-B235)
    - [LotsNestedMessage.B236](#google-protobuf-internal-LotsNestedMessage-B236)
    - [LotsNestedMessage.B237](#google-protobuf-internal-LotsNestedMessage-B237)
    - [LotsNestedMessage.B238](#google-protobuf-internal-LotsNestedMessage-B238)
    - [LotsNestedMessage.B239](#google-protobuf-internal-LotsNestedMessage-B239)
    - [LotsNestedMessage.B24](#google-protobuf-internal-LotsNestedMessage-B24)
    - [LotsNestedMessage.B240](#google-protobuf-internal-LotsNestedMessage-B240)
    - [LotsNestedMessage.B241](#google-protobuf-internal-LotsNestedMessage-B241)
    - [LotsNestedMessage.B242](#google-protobuf-internal-LotsNestedMessage-B242)
    - [LotsNestedMessage.B243](#google-protobuf-internal-LotsNestedMessage-B243)
    - [LotsNestedMessage.B244](#google-protobuf-internal-LotsNestedMessage-B244)
    - [LotsNestedMessage.B245](#google-protobuf-internal-LotsNestedMessage-B245)
    - [LotsNestedMessage.B246](#google-protobuf-internal-LotsNestedMessage-B246)
    - [LotsNestedMessage.B247](#google-protobuf-internal-LotsNestedMessage-B247)
    - [LotsNestedMessage.B248](#google-protobuf-internal-LotsNestedMessage-B248)
    - [LotsNestedMessage.B249](#google-protobuf-internal-LotsNestedMessage-B249)
    - [LotsNestedMessage.B25](#google-protobuf-internal-LotsNestedMessage-B25)
    - [LotsNestedMessage.B250](#google-protobuf-internal-LotsNestedMessage-B250)
    - [LotsNestedMessage.B251](#google-protobuf-internal-LotsNestedMessage-B251)
    - [LotsNestedMessage.B252](#google-protobuf-internal-LotsNestedMessage-B252)
    - [LotsNestedMessage.B253](#google-protobuf-internal-LotsNestedMessage-B253)
    - [LotsNestedMessage.B254](#google-protobuf-internal-LotsNestedMessage-B254)
    - [LotsNestedMessage.B255](#google-protobuf-internal-LotsNestedMessage-B255)
    - [LotsNestedMessage.B26](#google-protobuf-internal-LotsNestedMessage-B26)
    - [LotsNestedMessage.B27](#google-protobuf-internal-LotsNestedMessage-B27)
    - [LotsNestedMessage.B28](#google-protobuf-internal-LotsNestedMessage-B28)
    - [LotsNestedMessage.B29](#google-protobuf-internal-LotsNestedMessage-B29)
    - [LotsNestedMessage.B3](#google-protobuf-internal-LotsNestedMessage-B3)
    - [LotsNestedMessage.B30](#google-protobuf-internal-LotsNestedMessage-B30)
    - [LotsNestedMessage.B31](#google-protobuf-internal-LotsNestedMessage-B31)
    - [LotsNestedMessage.B32](#google-protobuf-internal-LotsNestedMessage-B32)
    - [LotsNestedMessage.B33](#google-protobuf-internal-LotsNestedMessage-B33)
    - [LotsNestedMessage.B34](#google-protobuf-internal-LotsNestedMessage-B34)
    - [LotsNestedMessage.B35](#google-protobuf-internal-LotsNestedMessage-B35)
    - [LotsNestedMessage.B36](#google-protobuf-internal-LotsNestedMessage-B36)
    - [LotsNestedMessage.B37](#google-protobuf-internal-LotsNestedMessage-B37)
    - [LotsNestedMessage.B38](#google-protobuf-internal-LotsNestedMessage-B38)
    - [LotsNestedMessage.B39](#google-protobuf-internal-LotsNestedMessage-B39)
    - [LotsNestedMessage.B4](#google-protobuf-internal-LotsNestedMessage-B4)
    - [LotsNestedMessage.B40](#google-protobuf-internal-LotsNestedMessage-B40)
    - [LotsNestedMessage.B41](#google-protobuf-internal-LotsNestedMessage-B41)
    - [LotsNestedMessage.B42](#google-protobuf-internal-LotsNestedMessage-B42)
    - [LotsNestedMessage.B43](#google-protobuf-internal-LotsNestedMessage-B43)
    - [LotsNestedMessage.B44](#google-protobuf-internal-LotsNestedMessage-B44)
    - [LotsNestedMessage.B45](#google-protobuf-internal-LotsNestedMessage-B45)
    - [LotsNestedMessage.B46](#google-protobuf-internal-LotsNestedMessage-B46)
    - [LotsNestedMessage.B47](#google-protobuf-internal-LotsNestedMessage-B47)
    - [LotsNestedMessage.B48](#google-protobuf-internal-LotsNestedMessage-B48)
    - [LotsNestedMessage.B49](#google-protobuf-internal-LotsNestedMessage-B49)
    - [LotsNestedMessage.B5](#google-protobuf-internal-LotsNestedMessage-B5)
    - [LotsNestedMessage.B50](#google-protobuf-internal-LotsNestedMessage-B50)
    - [LotsNestedMessage.B51](#google-protobuf-internal-LotsNestedMessage-B51)
    - [LotsNestedMessage.B52](#google-protobuf-internal-LotsNestedMessage-B52)
    - [LotsNestedMessage.B53](#google-protobuf-internal-LotsNestedMessage-B53)
    - [LotsNestedMessage.B54](#google-protobuf-internal-LotsNestedMessage-B54)
    - [LotsNestedMessage.B55](#google-protobuf-internal-LotsNestedMessage-B55)
    - [LotsNestedMessage.B56](#google-protobuf-internal-LotsNestedMessage-B56)
    - [LotsNestedMessage.B57](#google-protobuf-internal-LotsNestedMessage-B57)
    - [LotsNestedMessage.B58](#google-protobuf-internal-LotsNestedMessage-B58)
    - [LotsNestedMessage.B59](#google-protobuf-internal-LotsNestedMessage-B59)
    - [LotsNestedMessage.B6](#google-protobuf-internal-LotsNestedMessage-B6)
    - [LotsNestedMessage.B60](#google-protobuf-internal-LotsNestedMessage-B60)
    - [LotsNestedMessage.B61](#google-protobuf-internal-LotsNestedMessage-B61)
    - [LotsNestedMessage.B62](#google-protobuf-internal-LotsNestedMessage-B62)
    - [LotsNestedMessage.B63](#google-protobuf-internal-LotsNestedMessage-B63)
    - [LotsNestedMessage.B64](#google-protobuf-internal-LotsNestedMessage-B64)
    - [LotsNestedMessage.B65](#google-protobuf-internal-LotsNestedMessage-B65)
    - [LotsNestedMessage.B66](#google-protobuf-internal-LotsNestedMessage-B66)
    - [LotsNestedMessage.B67](#google-protobuf-internal-LotsNestedMessage-B67)
    - [LotsNestedMessage.B68](#google-protobuf-internal-LotsNestedMessage-B68)
    - [LotsNestedMessage.B69](#google-protobuf-internal-LotsNestedMessage-B69)
    - [LotsNestedMessage.B7](#google-protobuf-internal-LotsNestedMessage-B7)
    - [LotsNestedMessage.B70](#google-protobuf-internal-LotsNestedMessage-B70)
    - [LotsNestedMessage.B71](#google-protobuf-internal-LotsNestedMessage-B71)
    - [LotsNestedMessage.B72](#google-protobuf-internal-LotsNestedMessage-B72)
    - [LotsNestedMessage.B73](#google-protobuf-internal-LotsNestedMessage-B73)
    - [LotsNestedMessage.B74](#google-protobuf-internal-LotsNestedMessage-B74)
    - [LotsNestedMessage.B75](#google-protobuf-internal-LotsNestedMessage-B75)
    - [LotsNestedMessage.B76](#google-protobuf-internal-LotsNestedMessage-B76)
    - [LotsNestedMessage.B77](#google-protobuf-internal-LotsNestedMessage-B77)
    - [LotsNestedMessage.B78](#google-protobuf-internal-LotsNestedMessage-B78)
    - [LotsNestedMessage.B79](#google-protobuf-internal-LotsNestedMessage-B79)
    - [LotsNestedMessage.B8](#google-protobuf-internal-LotsNestedMessage-B8)
    - [LotsNestedMessage.B80](#google-protobuf-internal-LotsNestedMessage-B80)
    - [LotsNestedMessage.B81](#google-protobuf-internal-LotsNestedMessage-B81)
    - [LotsNestedMessage.B82](#google-protobuf-internal-LotsNestedMessage-B82)
    - [LotsNestedMessage.B83](#google-protobuf-internal-LotsNestedMessage-B83)
    - [LotsNestedMessage.B84](#google-protobuf-internal-LotsNestedMessage-B84)
    - [LotsNestedMessage.B85](#google-protobuf-internal-LotsNestedMessage-B85)
    - [LotsNestedMessage.B86](#google-protobuf-internal-LotsNestedMessage-B86)
    - [LotsNestedMessage.B87](#google-protobuf-internal-LotsNestedMessage-B87)
    - [LotsNestedMessage.B88](#google-protobuf-internal-LotsNestedMessage-B88)
    - [LotsNestedMessage.B89](#google-protobuf-internal-LotsNestedMessage-B89)
    - [LotsNestedMessage.B9](#google-protobuf-internal-LotsNestedMessage-B9)
    - [LotsNestedMessage.B90](#google-protobuf-internal-LotsNestedMessage-B90)
    - [LotsNestedMessage.B91](#google-protobuf-internal-LotsNestedMessage-B91)
    - [LotsNestedMessage.B92](#google-protobuf-internal-LotsNestedMessage-B92)
    - [LotsNestedMessage.B93](#google-protobuf-internal-LotsNestedMessage-B93)
    - [LotsNestedMessage.B94](#google-protobuf-internal-LotsNestedMessage-B94)
    - [LotsNestedMessage.B95](#google-protobuf-internal-LotsNestedMessage-B95)
    - [LotsNestedMessage.B96](#google-protobuf-internal-LotsNestedMessage-B96)
    - [LotsNestedMessage.B97](#google-protobuf-internal-LotsNestedMessage-B97)
    - [LotsNestedMessage.B98](#google-protobuf-internal-LotsNestedMessage-B98)
    - [LotsNestedMessage.B99](#google-protobuf-internal-LotsNestedMessage-B99)
    - [OutOfOrderFields](#google-protobuf-internal-OutOfOrderFields)
    - [TestFullKeyword](#google-protobuf-internal-TestFullKeyword)
    - [class](#google-protobuf-internal-class)
    - [class.try](#google-protobuf-internal-class-try)
  
    - [class.for](#google-protobuf-internal-class-for)
    - [is](#google-protobuf-internal-is)
  
    - [File-level Extensions](#python_google_protobuf_internal_more_messages-proto-extensions)
    - [File-level Extensions](#python_google_protobuf_internal_more_messages-proto-extensions)
    - [File-level Extensions](#python_google_protobuf_internal_more_messages-proto-extensions)
    - [File-level Extensions](#python_google_protobuf_internal_more_messages-proto-extensions)
  
- [Scalar Value Types](#scalar-value-types)



<a name="python_google_protobuf_internal_more_messages-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## python/google/protobuf/internal/more_messages.proto



<a name="google-protobuf-internal-ExtendClass"></a>

### ExtendClass





| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| return | int32 | class | 1002 | nested extension keyword |




<a name="google-protobuf-internal-LotsNestedMessage"></a>

### LotsNestedMessage







<a name="google-protobuf-internal-LotsNestedMessage-B0"></a>

### LotsNestedMessage.B0







<a name="google-protobuf-internal-LotsNestedMessage-B1"></a>

### LotsNestedMessage.B1







<a name="google-protobuf-internal-LotsNestedMessage-B10"></a>

### LotsNestedMessage.B10







<a name="google-protobuf-internal-LotsNestedMessage-B100"></a>

### LotsNestedMessage.B100







<a name="google-protobuf-internal-LotsNestedMessage-B101"></a>

### LotsNestedMessage.B101







<a name="google-protobuf-internal-LotsNestedMessage-B102"></a>

### LotsNestedMessage.B102







<a name="google-protobuf-internal-LotsNestedMessage-B103"></a>

### LotsNestedMessage.B103







<a name="google-protobuf-internal-LotsNestedMessage-B104"></a>

### LotsNestedMessage.B104







<a name="google-protobuf-internal-LotsNestedMessage-B105"></a>

### LotsNestedMessage.B105







<a name="google-protobuf-internal-LotsNestedMessage-B106"></a>

### LotsNestedMessage.B106







<a name="google-protobuf-internal-LotsNestedMessage-B107"></a>

### LotsNestedMessage.B107







<a name="google-protobuf-internal-LotsNestedMessage-B108"></a>

### LotsNestedMessage.B108







<a name="google-protobuf-internal-LotsNestedMessage-B109"></a>

### LotsNestedMessage.B109







<a name="google-protobuf-internal-LotsNestedMessage-B11"></a>

### LotsNestedMessage.B11







<a name="google-protobuf-internal-LotsNestedMessage-B110"></a>

### LotsNestedMessage.B110







<a name="google-protobuf-internal-LotsNestedMessage-B111"></a>

### LotsNestedMessage.B111







<a name="google-protobuf-internal-LotsNestedMessage-B112"></a>

### LotsNestedMessage.B112







<a name="google-protobuf-internal-LotsNestedMessage-B113"></a>

### LotsNestedMessage.B113







<a name="google-protobuf-internal-LotsNestedMessage-B114"></a>

### LotsNestedMessage.B114







<a name="google-protobuf-internal-LotsNestedMessage-B115"></a>

### LotsNestedMessage.B115







<a name="google-protobuf-internal-LotsNestedMessage-B116"></a>

### LotsNestedMessage.B116







<a name="google-protobuf-internal-LotsNestedMessage-B117"></a>

### LotsNestedMessage.B117







<a name="google-protobuf-internal-LotsNestedMessage-B118"></a>

### LotsNestedMessage.B118







<a name="google-protobuf-internal-LotsNestedMessage-B119"></a>

### LotsNestedMessage.B119







<a name="google-protobuf-internal-LotsNestedMessage-B12"></a>

### LotsNestedMessage.B12







<a name="google-protobuf-internal-LotsNestedMessage-B120"></a>

### LotsNestedMessage.B120







<a name="google-protobuf-internal-LotsNestedMessage-B121"></a>

### LotsNestedMessage.B121







<a name="google-protobuf-internal-LotsNestedMessage-B122"></a>

### LotsNestedMessage.B122







<a name="google-protobuf-internal-LotsNestedMessage-B123"></a>

### LotsNestedMessage.B123







<a name="google-protobuf-internal-LotsNestedMessage-B124"></a>

### LotsNestedMessage.B124







<a name="google-protobuf-internal-LotsNestedMessage-B125"></a>

### LotsNestedMessage.B125







<a name="google-protobuf-internal-LotsNestedMessage-B126"></a>

### LotsNestedMessage.B126







<a name="google-protobuf-internal-LotsNestedMessage-B127"></a>

### LotsNestedMessage.B127







<a name="google-protobuf-internal-LotsNestedMessage-B128"></a>

### LotsNestedMessage.B128







<a name="google-protobuf-internal-LotsNestedMessage-B129"></a>

### LotsNestedMessage.B129







<a name="google-protobuf-internal-LotsNestedMessage-B13"></a>

### LotsNestedMessage.B13







<a name="google-protobuf-internal-LotsNestedMessage-B130"></a>

### LotsNestedMessage.B130







<a name="google-protobuf-internal-LotsNestedMessage-B131"></a>

### LotsNestedMessage.B131







<a name="google-protobuf-internal-LotsNestedMessage-B132"></a>

### LotsNestedMessage.B132







<a name="google-protobuf-internal-LotsNestedMessage-B133"></a>

### LotsNestedMessage.B133







<a name="google-protobuf-internal-LotsNestedMessage-B134"></a>

### LotsNestedMessage.B134







<a name="google-protobuf-internal-LotsNestedMessage-B135"></a>

### LotsNestedMessage.B135







<a name="google-protobuf-internal-LotsNestedMessage-B136"></a>

### LotsNestedMessage.B136







<a name="google-protobuf-internal-LotsNestedMessage-B137"></a>

### LotsNestedMessage.B137







<a name="google-protobuf-internal-LotsNestedMessage-B138"></a>

### LotsNestedMessage.B138







<a name="google-protobuf-internal-LotsNestedMessage-B139"></a>

### LotsNestedMessage.B139







<a name="google-protobuf-internal-LotsNestedMessage-B14"></a>

### LotsNestedMessage.B14







<a name="google-protobuf-internal-LotsNestedMessage-B140"></a>

### LotsNestedMessage.B140







<a name="google-protobuf-internal-LotsNestedMessage-B141"></a>

### LotsNestedMessage.B141







<a name="google-protobuf-internal-LotsNestedMessage-B142"></a>

### LotsNestedMessage.B142







<a name="google-protobuf-internal-LotsNestedMessage-B143"></a>

### LotsNestedMessage.B143







<a name="google-protobuf-internal-LotsNestedMessage-B144"></a>

### LotsNestedMessage.B144







<a name="google-protobuf-internal-LotsNestedMessage-B145"></a>

### LotsNestedMessage.B145







<a name="google-protobuf-internal-LotsNestedMessage-B146"></a>

### LotsNestedMessage.B146







<a name="google-protobuf-internal-LotsNestedMessage-B147"></a>

### LotsNestedMessage.B147







<a name="google-protobuf-internal-LotsNestedMessage-B148"></a>

### LotsNestedMessage.B148







<a name="google-protobuf-internal-LotsNestedMessage-B149"></a>

### LotsNestedMessage.B149







<a name="google-protobuf-internal-LotsNestedMessage-B15"></a>

### LotsNestedMessage.B15







<a name="google-protobuf-internal-LotsNestedMessage-B150"></a>

### LotsNestedMessage.B150







<a name="google-protobuf-internal-LotsNestedMessage-B151"></a>

### LotsNestedMessage.B151







<a name="google-protobuf-internal-LotsNestedMessage-B152"></a>

### LotsNestedMessage.B152







<a name="google-protobuf-internal-LotsNestedMessage-B153"></a>

### LotsNestedMessage.B153







<a name="google-protobuf-internal-LotsNestedMessage-B154"></a>

### LotsNestedMessage.B154







<a name="google-protobuf-internal-LotsNestedMessage-B155"></a>

### LotsNestedMessage.B155







<a name="google-protobuf-internal-LotsNestedMessage-B156"></a>

### LotsNestedMessage.B156







<a name="google-protobuf-internal-LotsNestedMessage-B157"></a>

### LotsNestedMessage.B157







<a name="google-protobuf-internal-LotsNestedMessage-B158"></a>

### LotsNestedMessage.B158







<a name="google-protobuf-internal-LotsNestedMessage-B159"></a>

### LotsNestedMessage.B159







<a name="google-protobuf-internal-LotsNestedMessage-B16"></a>

### LotsNestedMessage.B16







<a name="google-protobuf-internal-LotsNestedMessage-B160"></a>

### LotsNestedMessage.B160







<a name="google-protobuf-internal-LotsNestedMessage-B161"></a>

### LotsNestedMessage.B161







<a name="google-protobuf-internal-LotsNestedMessage-B162"></a>

### LotsNestedMessage.B162







<a name="google-protobuf-internal-LotsNestedMessage-B163"></a>

### LotsNestedMessage.B163







<a name="google-protobuf-internal-LotsNestedMessage-B164"></a>

### LotsNestedMessage.B164







<a name="google-protobuf-internal-LotsNestedMessage-B165"></a>

### LotsNestedMessage.B165







<a name="google-protobuf-internal-LotsNestedMessage-B166"></a>

### LotsNestedMessage.B166







<a name="google-protobuf-internal-LotsNestedMessage-B167"></a>

### LotsNestedMessage.B167







<a name="google-protobuf-internal-LotsNestedMessage-B168"></a>

### LotsNestedMessage.B168







<a name="google-protobuf-internal-LotsNestedMessage-B169"></a>

### LotsNestedMessage.B169







<a name="google-protobuf-internal-LotsNestedMessage-B17"></a>

### LotsNestedMessage.B17







<a name="google-protobuf-internal-LotsNestedMessage-B170"></a>

### LotsNestedMessage.B170







<a name="google-protobuf-internal-LotsNestedMessage-B171"></a>

### LotsNestedMessage.B171







<a name="google-protobuf-internal-LotsNestedMessage-B172"></a>

### LotsNestedMessage.B172







<a name="google-protobuf-internal-LotsNestedMessage-B173"></a>

### LotsNestedMessage.B173







<a name="google-protobuf-internal-LotsNestedMessage-B174"></a>

### LotsNestedMessage.B174







<a name="google-protobuf-internal-LotsNestedMessage-B175"></a>

### LotsNestedMessage.B175







<a name="google-protobuf-internal-LotsNestedMessage-B176"></a>

### LotsNestedMessage.B176







<a name="google-protobuf-internal-LotsNestedMessage-B177"></a>

### LotsNestedMessage.B177







<a name="google-protobuf-internal-LotsNestedMessage-B178"></a>

### LotsNestedMessage.B178







<a name="google-protobuf-internal-LotsNestedMessage-B179"></a>

### LotsNestedMessage.B179







<a name="google-protobuf-internal-LotsNestedMessage-B18"></a>

### LotsNestedMessage.B18







<a name="google-protobuf-internal-LotsNestedMessage-B180"></a>

### LotsNestedMessage.B180







<a name="google-protobuf-internal-LotsNestedMessage-B181"></a>

### LotsNestedMessage.B181







<a name="google-protobuf-internal-LotsNestedMessage-B182"></a>

### LotsNestedMessage.B182







<a name="google-protobuf-internal-LotsNestedMessage-B183"></a>

### LotsNestedMessage.B183







<a name="google-protobuf-internal-LotsNestedMessage-B184"></a>

### LotsNestedMessage.B184







<a name="google-protobuf-internal-LotsNestedMessage-B185"></a>

### LotsNestedMessage.B185







<a name="google-protobuf-internal-LotsNestedMessage-B186"></a>

### LotsNestedMessage.B186







<a name="google-protobuf-internal-LotsNestedMessage-B187"></a>

### LotsNestedMessage.B187







<a name="google-protobuf-internal-LotsNestedMessage-B188"></a>

### LotsNestedMessage.B188







<a name="google-protobuf-internal-LotsNestedMessage-B189"></a>

### LotsNestedMessage.B189







<a name="google-protobuf-internal-LotsNestedMessage-B19"></a>

### LotsNestedMessage.B19







<a name="google-protobuf-internal-LotsNestedMessage-B190"></a>

### LotsNestedMessage.B190







<a name="google-protobuf-internal-LotsNestedMessage-B191"></a>

### LotsNestedMessage.B191







<a name="google-protobuf-internal-LotsNestedMessage-B192"></a>

### LotsNestedMessage.B192







<a name="google-protobuf-internal-LotsNestedMessage-B193"></a>

### LotsNestedMessage.B193







<a name="google-protobuf-internal-LotsNestedMessage-B194"></a>

### LotsNestedMessage.B194







<a name="google-protobuf-internal-LotsNestedMessage-B195"></a>

### LotsNestedMessage.B195







<a name="google-protobuf-internal-LotsNestedMessage-B196"></a>

### LotsNestedMessage.B196







<a name="google-protobuf-internal-LotsNestedMessage-B197"></a>

### LotsNestedMessage.B197







<a name="google-protobuf-internal-LotsNestedMessage-B198"></a>

### LotsNestedMessage.B198







<a name="google-protobuf-internal-LotsNestedMessage-B199"></a>

### LotsNestedMessage.B199







<a name="google-protobuf-internal-LotsNestedMessage-B2"></a>

### LotsNestedMessage.B2







<a name="google-protobuf-internal-LotsNestedMessage-B20"></a>

### LotsNestedMessage.B20







<a name="google-protobuf-internal-LotsNestedMessage-B200"></a>

### LotsNestedMessage.B200







<a name="google-protobuf-internal-LotsNestedMessage-B201"></a>

### LotsNestedMessage.B201







<a name="google-protobuf-internal-LotsNestedMessage-B202"></a>

### LotsNestedMessage.B202







<a name="google-protobuf-internal-LotsNestedMessage-B203"></a>

### LotsNestedMessage.B203







<a name="google-protobuf-internal-LotsNestedMessage-B204"></a>

### LotsNestedMessage.B204







<a name="google-protobuf-internal-LotsNestedMessage-B205"></a>

### LotsNestedMessage.B205







<a name="google-protobuf-internal-LotsNestedMessage-B206"></a>

### LotsNestedMessage.B206







<a name="google-protobuf-internal-LotsNestedMessage-B207"></a>

### LotsNestedMessage.B207







<a name="google-protobuf-internal-LotsNestedMessage-B208"></a>

### LotsNestedMessage.B208







<a name="google-protobuf-internal-LotsNestedMessage-B209"></a>

### LotsNestedMessage.B209







<a name="google-protobuf-internal-LotsNestedMessage-B21"></a>

### LotsNestedMessage.B21







<a name="google-protobuf-internal-LotsNestedMessage-B210"></a>

### LotsNestedMessage.B210







<a name="google-protobuf-internal-LotsNestedMessage-B211"></a>

### LotsNestedMessage.B211







<a name="google-protobuf-internal-LotsNestedMessage-B212"></a>

### LotsNestedMessage.B212







<a name="google-protobuf-internal-LotsNestedMessage-B213"></a>

### LotsNestedMessage.B213







<a name="google-protobuf-internal-LotsNestedMessage-B214"></a>

### LotsNestedMessage.B214







<a name="google-protobuf-internal-LotsNestedMessage-B215"></a>

### LotsNestedMessage.B215







<a name="google-protobuf-internal-LotsNestedMessage-B216"></a>

### LotsNestedMessage.B216







<a name="google-protobuf-internal-LotsNestedMessage-B217"></a>

### LotsNestedMessage.B217







<a name="google-protobuf-internal-LotsNestedMessage-B218"></a>

### LotsNestedMessage.B218







<a name="google-protobuf-internal-LotsNestedMessage-B219"></a>

### LotsNestedMessage.B219







<a name="google-protobuf-internal-LotsNestedMessage-B22"></a>

### LotsNestedMessage.B22







<a name="google-protobuf-internal-LotsNestedMessage-B220"></a>

### LotsNestedMessage.B220







<a name="google-protobuf-internal-LotsNestedMessage-B221"></a>

### LotsNestedMessage.B221







<a name="google-protobuf-internal-LotsNestedMessage-B222"></a>

### LotsNestedMessage.B222







<a name="google-protobuf-internal-LotsNestedMessage-B223"></a>

### LotsNestedMessage.B223







<a name="google-protobuf-internal-LotsNestedMessage-B224"></a>

### LotsNestedMessage.B224







<a name="google-protobuf-internal-LotsNestedMessage-B225"></a>

### LotsNestedMessage.B225







<a name="google-protobuf-internal-LotsNestedMessage-B226"></a>

### LotsNestedMessage.B226







<a name="google-protobuf-internal-LotsNestedMessage-B227"></a>

### LotsNestedMessage.B227







<a name="google-protobuf-internal-LotsNestedMessage-B228"></a>

### LotsNestedMessage.B228







<a name="google-protobuf-internal-LotsNestedMessage-B229"></a>

### LotsNestedMessage.B229







<a name="google-protobuf-internal-LotsNestedMessage-B23"></a>

### LotsNestedMessage.B23







<a name="google-protobuf-internal-LotsNestedMessage-B230"></a>

### LotsNestedMessage.B230







<a name="google-protobuf-internal-LotsNestedMessage-B231"></a>

### LotsNestedMessage.B231







<a name="google-protobuf-internal-LotsNestedMessage-B232"></a>

### LotsNestedMessage.B232







<a name="google-protobuf-internal-LotsNestedMessage-B233"></a>

### LotsNestedMessage.B233







<a name="google-protobuf-internal-LotsNestedMessage-B234"></a>

### LotsNestedMessage.B234







<a name="google-protobuf-internal-LotsNestedMessage-B235"></a>

### LotsNestedMessage.B235







<a name="google-protobuf-internal-LotsNestedMessage-B236"></a>

### LotsNestedMessage.B236







<a name="google-protobuf-internal-LotsNestedMessage-B237"></a>

### LotsNestedMessage.B237







<a name="google-protobuf-internal-LotsNestedMessage-B238"></a>

### LotsNestedMessage.B238







<a name="google-protobuf-internal-LotsNestedMessage-B239"></a>

### LotsNestedMessage.B239







<a name="google-protobuf-internal-LotsNestedMessage-B24"></a>

### LotsNestedMessage.B24







<a name="google-protobuf-internal-LotsNestedMessage-B240"></a>

### LotsNestedMessage.B240







<a name="google-protobuf-internal-LotsNestedMessage-B241"></a>

### LotsNestedMessage.B241







<a name="google-protobuf-internal-LotsNestedMessage-B242"></a>

### LotsNestedMessage.B242







<a name="google-protobuf-internal-LotsNestedMessage-B243"></a>

### LotsNestedMessage.B243







<a name="google-protobuf-internal-LotsNestedMessage-B244"></a>

### LotsNestedMessage.B244







<a name="google-protobuf-internal-LotsNestedMessage-B245"></a>

### LotsNestedMessage.B245







<a name="google-protobuf-internal-LotsNestedMessage-B246"></a>

### LotsNestedMessage.B246







<a name="google-protobuf-internal-LotsNestedMessage-B247"></a>

### LotsNestedMessage.B247







<a name="google-protobuf-internal-LotsNestedMessage-B248"></a>

### LotsNestedMessage.B248







<a name="google-protobuf-internal-LotsNestedMessage-B249"></a>

### LotsNestedMessage.B249







<a name="google-protobuf-internal-LotsNestedMessage-B25"></a>

### LotsNestedMessage.B25







<a name="google-protobuf-internal-LotsNestedMessage-B250"></a>

### LotsNestedMessage.B250







<a name="google-protobuf-internal-LotsNestedMessage-B251"></a>

### LotsNestedMessage.B251







<a name="google-protobuf-internal-LotsNestedMessage-B252"></a>

### LotsNestedMessage.B252







<a name="google-protobuf-internal-LotsNestedMessage-B253"></a>

### LotsNestedMessage.B253







<a name="google-protobuf-internal-LotsNestedMessage-B254"></a>

### LotsNestedMessage.B254







<a name="google-protobuf-internal-LotsNestedMessage-B255"></a>

### LotsNestedMessage.B255







<a name="google-protobuf-internal-LotsNestedMessage-B26"></a>

### LotsNestedMessage.B26







<a name="google-protobuf-internal-LotsNestedMessage-B27"></a>

### LotsNestedMessage.B27







<a name="google-protobuf-internal-LotsNestedMessage-B28"></a>

### LotsNestedMessage.B28







<a name="google-protobuf-internal-LotsNestedMessage-B29"></a>

### LotsNestedMessage.B29







<a name="google-protobuf-internal-LotsNestedMessage-B3"></a>

### LotsNestedMessage.B3







<a name="google-protobuf-internal-LotsNestedMessage-B30"></a>

### LotsNestedMessage.B30







<a name="google-protobuf-internal-LotsNestedMessage-B31"></a>

### LotsNestedMessage.B31







<a name="google-protobuf-internal-LotsNestedMessage-B32"></a>

### LotsNestedMessage.B32







<a name="google-protobuf-internal-LotsNestedMessage-B33"></a>

### LotsNestedMessage.B33







<a name="google-protobuf-internal-LotsNestedMessage-B34"></a>

### LotsNestedMessage.B34







<a name="google-protobuf-internal-LotsNestedMessage-B35"></a>

### LotsNestedMessage.B35







<a name="google-protobuf-internal-LotsNestedMessage-B36"></a>

### LotsNestedMessage.B36







<a name="google-protobuf-internal-LotsNestedMessage-B37"></a>

### LotsNestedMessage.B37







<a name="google-protobuf-internal-LotsNestedMessage-B38"></a>

### LotsNestedMessage.B38







<a name="google-protobuf-internal-LotsNestedMessage-B39"></a>

### LotsNestedMessage.B39







<a name="google-protobuf-internal-LotsNestedMessage-B4"></a>

### LotsNestedMessage.B4







<a name="google-protobuf-internal-LotsNestedMessage-B40"></a>

### LotsNestedMessage.B40







<a name="google-protobuf-internal-LotsNestedMessage-B41"></a>

### LotsNestedMessage.B41







<a name="google-protobuf-internal-LotsNestedMessage-B42"></a>

### LotsNestedMessage.B42







<a name="google-protobuf-internal-LotsNestedMessage-B43"></a>

### LotsNestedMessage.B43







<a name="google-protobuf-internal-LotsNestedMessage-B44"></a>

### LotsNestedMessage.B44







<a name="google-protobuf-internal-LotsNestedMessage-B45"></a>

### LotsNestedMessage.B45







<a name="google-protobuf-internal-LotsNestedMessage-B46"></a>

### LotsNestedMessage.B46







<a name="google-protobuf-internal-LotsNestedMessage-B47"></a>

### LotsNestedMessage.B47







<a name="google-protobuf-internal-LotsNestedMessage-B48"></a>

### LotsNestedMessage.B48







<a name="google-protobuf-internal-LotsNestedMessage-B49"></a>

### LotsNestedMessage.B49







<a name="google-protobuf-internal-LotsNestedMessage-B5"></a>

### LotsNestedMessage.B5







<a name="google-protobuf-internal-LotsNestedMessage-B50"></a>

### LotsNestedMessage.B50







<a name="google-protobuf-internal-LotsNestedMessage-B51"></a>

### LotsNestedMessage.B51







<a name="google-protobuf-internal-LotsNestedMessage-B52"></a>

### LotsNestedMessage.B52







<a name="google-protobuf-internal-LotsNestedMessage-B53"></a>

### LotsNestedMessage.B53







<a name="google-protobuf-internal-LotsNestedMessage-B54"></a>

### LotsNestedMessage.B54







<a name="google-protobuf-internal-LotsNestedMessage-B55"></a>

### LotsNestedMessage.B55







<a name="google-protobuf-internal-LotsNestedMessage-B56"></a>

### LotsNestedMessage.B56







<a name="google-protobuf-internal-LotsNestedMessage-B57"></a>

### LotsNestedMessage.B57







<a name="google-protobuf-internal-LotsNestedMessage-B58"></a>

### LotsNestedMessage.B58







<a name="google-protobuf-internal-LotsNestedMessage-B59"></a>

### LotsNestedMessage.B59







<a name="google-protobuf-internal-LotsNestedMessage-B6"></a>

### LotsNestedMessage.B6







<a name="google-protobuf-internal-LotsNestedMessage-B60"></a>

### LotsNestedMessage.B60







<a name="google-protobuf-internal-LotsNestedMessage-B61"></a>

### LotsNestedMessage.B61







<a name="google-protobuf-internal-LotsNestedMessage-B62"></a>

### LotsNestedMessage.B62







<a name="google-protobuf-internal-LotsNestedMessage-B63"></a>

### LotsNestedMessage.B63







<a name="google-protobuf-internal-LotsNestedMessage-B64"></a>

### LotsNestedMessage.B64







<a name="google-protobuf-internal-LotsNestedMessage-B65"></a>

### LotsNestedMessage.B65







<a name="google-protobuf-internal-LotsNestedMessage-B66"></a>

### LotsNestedMessage.B66







<a name="google-protobuf-internal-LotsNestedMessage-B67"></a>

### LotsNestedMessage.B67







<a name="google-protobuf-internal-LotsNestedMessage-B68"></a>

### LotsNestedMessage.B68







<a name="google-protobuf-internal-LotsNestedMessage-B69"></a>

### LotsNestedMessage.B69







<a name="google-protobuf-internal-LotsNestedMessage-B7"></a>

### LotsNestedMessage.B7







<a name="google-protobuf-internal-LotsNestedMessage-B70"></a>

### LotsNestedMessage.B70







<a name="google-protobuf-internal-LotsNestedMessage-B71"></a>

### LotsNestedMessage.B71







<a name="google-protobuf-internal-LotsNestedMessage-B72"></a>

### LotsNestedMessage.B72







<a name="google-protobuf-internal-LotsNestedMessage-B73"></a>

### LotsNestedMessage.B73







<a name="google-protobuf-internal-LotsNestedMessage-B74"></a>

### LotsNestedMessage.B74







<a name="google-protobuf-internal-LotsNestedMessage-B75"></a>

### LotsNestedMessage.B75







<a name="google-protobuf-internal-LotsNestedMessage-B76"></a>

### LotsNestedMessage.B76







<a name="google-protobuf-internal-LotsNestedMessage-B77"></a>

### LotsNestedMessage.B77







<a name="google-protobuf-internal-LotsNestedMessage-B78"></a>

### LotsNestedMessage.B78







<a name="google-protobuf-internal-LotsNestedMessage-B79"></a>

### LotsNestedMessage.B79







<a name="google-protobuf-internal-LotsNestedMessage-B8"></a>

### LotsNestedMessage.B8







<a name="google-protobuf-internal-LotsNestedMessage-B80"></a>

### LotsNestedMessage.B80







<a name="google-protobuf-internal-LotsNestedMessage-B81"></a>

### LotsNestedMessage.B81







<a name="google-protobuf-internal-LotsNestedMessage-B82"></a>

### LotsNestedMessage.B82







<a name="google-protobuf-internal-LotsNestedMessage-B83"></a>

### LotsNestedMessage.B83







<a name="google-protobuf-internal-LotsNestedMessage-B84"></a>

### LotsNestedMessage.B84







<a name="google-protobuf-internal-LotsNestedMessage-B85"></a>

### LotsNestedMessage.B85







<a name="google-protobuf-internal-LotsNestedMessage-B86"></a>

### LotsNestedMessage.B86







<a name="google-protobuf-internal-LotsNestedMessage-B87"></a>

### LotsNestedMessage.B87







<a name="google-protobuf-internal-LotsNestedMessage-B88"></a>

### LotsNestedMessage.B88







<a name="google-protobuf-internal-LotsNestedMessage-B89"></a>

### LotsNestedMessage.B89







<a name="google-protobuf-internal-LotsNestedMessage-B9"></a>

### LotsNestedMessage.B9







<a name="google-protobuf-internal-LotsNestedMessage-B90"></a>

### LotsNestedMessage.B90







<a name="google-protobuf-internal-LotsNestedMessage-B91"></a>

### LotsNestedMessage.B91







<a name="google-protobuf-internal-LotsNestedMessage-B92"></a>

### LotsNestedMessage.B92







<a name="google-protobuf-internal-LotsNestedMessage-B93"></a>

### LotsNestedMessage.B93







<a name="google-protobuf-internal-LotsNestedMessage-B94"></a>

### LotsNestedMessage.B94







<a name="google-protobuf-internal-LotsNestedMessage-B95"></a>

### LotsNestedMessage.B95







<a name="google-protobuf-internal-LotsNestedMessage-B96"></a>

### LotsNestedMessage.B96







<a name="google-protobuf-internal-LotsNestedMessage-B97"></a>

### LotsNestedMessage.B97







<a name="google-protobuf-internal-LotsNestedMessage-B98"></a>

### LotsNestedMessage.B98







<a name="google-protobuf-internal-LotsNestedMessage-B99"></a>

### LotsNestedMessage.B99







<a name="google-protobuf-internal-OutOfOrderFields"></a>

### OutOfOrderFields
A message where tag numbers are listed out of order, to allow us to test our
canonicalization of serialized output, which should always be in tag order.
We also mix in some extensions for extra fun.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| optional_sint32 | [sint32](#sint32) | optional |  |
| optional_uint32 | [uint32](#uint32) | optional |  |
| optional_int32 | [int32](#int32) | optional |  |






<a name="google-protobuf-internal-TestFullKeyword"></a>

### TestFullKeyword



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field1 | [OutOfOrderFields](#google-protobuf-internal-OutOfOrderFields) | optional |  |
| field2 | [class](#google-protobuf-internal-class) | optional |  |






<a name="google-protobuf-internal-class"></a>

### class
message keyword


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| int_field | [int32](#int32) | optional |  |
| if | [int32](#int32) | optional | field keyword |
| as | [is](#google-protobuf-internal-is) | optional | enum field keyword |
| enum_field | [is](#google-protobuf-internal-is) | optional |  |
| nested_enum_field | [class.for](#google-protobuf-internal-class-for) | optional |  |
| nested_message | [class.try](#google-protobuf-internal-class-try) | optional |  |






<a name="google-protobuf-internal-class-try"></a>

### class.try



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| field | [int32](#int32) | optional |  |





 


<a name="google-protobuf-internal-class-for"></a>

### class.for
nested enum keyword

| Name | Number | Description |
| ---- | ------ | ----------- |
| default | 0 |  |
| True | 1 | nested enum value keyword |



<a name="google-protobuf-internal-is"></a>

### is
top level enum keyword

| Name | Number | Description |
| ---- | ------ | ----------- |
| default | 0 |  |
| else | 1 | top level enum value keyword |


 


<a name="python_google_protobuf_internal_more_messages-proto-extensions"></a>

### File-level Extensions
| Extension | Type | Base | Number | Description |
| --------- | ---- | ---- | ------ | ----------- |
| optional_int64 | int64 | OutOfOrderFields | 2 |  |
| optional_uint64 | uint64 | OutOfOrderFields | 4 |  |
| continue | int32 | class | 1001 | top level extension keyword |
| with | int32 | class.try | 1001 |  |

 

 



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

