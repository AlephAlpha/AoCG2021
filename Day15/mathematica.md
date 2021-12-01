# [Wolfram Language (Mathematica)], 86 bytes

    (Clear@a;d=p=a@_0;a@0=1;(While[a[p+=#]>0d++];a@p=1)&/@(I^ToCharacterCode@#~Mod~11);d)&

[Try it online!][TIO-kwnn8v4a]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwnn8v4a]: https://tio.run/##LYlNC4MgHMa/iiRE0UZ5NkXotMNgh8EOYuNPGga1QsTLWF/d1drv4YHnZQJvzQR@6CD2iMWsGQ04AVSzhYF4VhRExQjNHnYYjQS5FAwrXumiUNu1MJKnpcgu7X1uLDjovHHNrI3A63XWKyE51Xkab254eYnRmaNeYqVQikqB3kloDyUnlLQ81Jv3yH/UB/8hhLCXT/wC "Wolfram Language (Mathematica) – Try It Online"