# [Wolfram Language (Mathematica)], 107 bytes

    -Max[Count@4/@Select[Tuples[Range@4,l=Length[s=ToCharacterCode@#~Mod~11]],0!=##&@@Accumulate[I^(s+#)]&]]+l&

[Try it online!][TIO-kwq4qgud]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwq4qgud]: https://tio.run/##LcfdCoIwGIDhW1kORqFigoduLDwKEqI8GxPG/PyBOUOnBJG3bhQdvDy8vXIt9Mp1Wm01oluYq6fIhtk6nkT8Dga0E8X8MDCJm7IN8CQw9AK2ca2YaDFkrRqVdjBmQwUcr/lQrXEsZXDcUYwJ5yet5342yoE4l/vJxwdJpPQN2a5jZ53AKGSoFlhKRFDE0csrS8aWJU29AHksZX9@W6YL@@a9tw8 "Wolfram Language (Mathematica) – Try It Online"