# [Wolfram Language (Mathematica)], 102 bytes

    Pick[#,Total[Outer[Boole[#==#2||#==Reverse@#2]&,e={#[[1]],Last@#,First/@#,Last/@#}&/@#,e,2],{2,4}],8]&

[Try it online!][TIO-kxmmlyxv]

A port of [@Neil's answer](https://codegolf.stackexchange.com/a/240143/9288).

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/

[TIO-kxmmlyxv]: https://tio.run/##jVSxasMwEN3zFQaBJ0HvTIcuBtOhU6EhdBMaRFCoaVKDrWZR/O2u3TT1ST65BWNJT@fnp3d3Ohn3Zk/G1XszHLJy2Nb7dyXka@PMUb18Otuqx6Y5WiXKUhSXyzjs7Nm2na1EoXNpSy@UQq3ls@lcJeRT3XbubpxM63Hs82lhZaGlL@R9r@WDzodtW384dVBC6zyrNt57kBnenmney02WeSTotHFF4Rry/Q5ifzeCWCQoRgw3dIL9TAGUghIDSxyjGKGUFyIRM8@PCKDf/y0iPAdxDZb@ME5E0mAWETiXCCZoMnVrDAy6SAeunCNJwUjj6weXqYM4Hfzp1jIKUbHxJYgpJ4g0KgKWZjJO/Ot3fLmmGGhhMhSMmcjGRu3MSOO7DvnCjEXw/uAySUzjJm8aDEX0wxc "Wolfram Language (Mathematica) – Try It Online"