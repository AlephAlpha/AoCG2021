# [Wolfram Language (Mathematica)], 95 bytes

    Min[p=Position;Count[Or@@@#,1<0]&/@Outer[Det@{u=#-#3,v=#3-#2}==0<u.v&,#~p~1,#~p~2,p[#,1|2],1]]&

[Try it online!][TIO-kxidxr37]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kxidxr37]: https://tio.run/##lU6xCoMwFNz9igcBp1iTONaUQLsW3UMGKUozVMVGF6u/blNjFZdC4XjcO@6Oe2Tmnj8yo2/ZVACfrrqUNU@rpza6Ko/nqi2NTBohBMI0JsoPRdKavJGX3Ii@5ShAEe44igLEBs5J3B46H6OxHul8Ga6lTb6YwlQpf0obbQsRBCcoJFIKfAiFB33f02HAHlhGMViw78ssd5gF@EdYO4l7MZDF8qEz6JahS2Z1OBPbDyM7F3Mluyr6S2PbhnWUWzpMbw "Wolfram Language (Mathematica) – Try It Online"