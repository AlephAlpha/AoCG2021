# [Wolfram Language (Mathematica)], 41 bytes

    FreeQ[Or@@StringLength@#/. 1||1->3,1||2]&

[Try it online!][TIO-kx04lwn5]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kx04lwn5]: https://tio.run/##y00syUjNTSzJTE78n6Zg@9@tKDU1MNq/yMEhuKQoMy/dJzUvvSTDQVlfT8GwpsZQ185YB0gbxar9DwBKl0QrK@jaKaRFK8fGKqgp6DtwVVfX6nApVCsFK0HpcCjDT0lHQckVRPiFg0lXmARYMBhChiMpgGsIBhF4zIGrw2YkmjHINqAYCRSqrf0PAA "Wolfram Language (Mathematica) – Try It Online"