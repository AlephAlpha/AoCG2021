# [Wolfram Language (Mathematica)], 79 bytes

    (a[d=p=0]=0Clear@a;(a@p=0While[a[p+=#]<++d])&/@(I^ToCharacterCode@#~Mod~11);d)&

[Try it online!][TIO-kx7b91si]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kx7b91si]: https://tio.run/##LYhBCoMwFESv8jEgES3qWiMBV10Uuih0ESJ8TCSCVgkhm1KvnmrtGwZm3ozO6Bnd2GMYgAWKQrGVFZIV7aTRcqwo8l08zThpgWJNGZF1miqZxDmn1@6xtAYt9k7bdlGak@22qK0sk0olcbjb8eUEgUsDgyBSQgw5h3fkuzNRBlHX@HrvMZsf9clfeO@P8wlf "Wolfram Language (Mathematica) – Try It Online"