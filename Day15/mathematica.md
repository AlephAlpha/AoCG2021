# [Wolfram Language (Mathematica)], 77 bytes

    (Clear@a;c=p=0;a@_=-1;Do[p+={1,1-I,-I,-1,I-1,I}[[Mod[c+=a@p*=-1,6,1]]],#];c)&

[Try it online!][TIO-kwm1pbci]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwm1pbci]: https://tio.run/##y00syUjNTSzJTE78n6Zg@1/DOSc1scgh0TrZtsDWwDrRId5W19DaJT@6QNu22lDHUNdTB4QMdTxBuDY62jc/JTpZ2zbRoUALqFLHTMcwNjZWRznWOllT7T9QX0BRZl5JdFp0HlBUoTpPR8FAR8HIoDb2PwA "Wolfram Language (Mathematica) – Try It Online"