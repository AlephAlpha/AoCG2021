# [Wolfram Language (Mathematica)], 55 bytes

    Min[Tr/@Abs@Fold[#.Most@s+#2s&,s=ReIm@{1-I,1,I};0s,#]]&

[Try it online!][TIO-kwcxm8wp]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwcxm8wp]: https://tio.run/##y00syUjNTSzJTE78n6Zg@983My86pEjfwTGp2MEtPyclWlnPN7@4xKFYW9moWE2n2DYo1TPXodpQ11PHUMez1tqgWEc5Nlbtf0BRZl5JdLVyrYKunUJaNFBMQU1B30GhurpWR6HaUEcBhBBMAx0FIyjPCMyDICOEIiDTWEfBpLb2PwA "Wolfram Language (Mathematica) – Try It Online"