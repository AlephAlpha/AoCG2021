# [Wolfram Language (Mathematica)], 103 bytes

    Ordering[i=1;s=I^ToCharacterCode@#~Mod~11;-Length[{0}⋃##]&@@Accumulate@Partition[s,i,i++,1,0]&/@s,1]&

[Try it online!][TIO-kwlulp36]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwlulp36]: https://tio.run/##NY0xCoMwAEWvEhJwMUUzqyHFqdBSh24hgaBRA1UhxiyiS8feshexWuh/y3vT75RrdaecKdVWg2y720pb0zfcZCQZs4t8DHmrrCqdtvlQaYbW21CthCSnq@4b1/I5Xj7vF0IiYOxcllM3PZXTrFDWGWeGno/YYBOGmOBYBBEbMRHBVuwnjiNwoqDmSAgQgIiBGdJjEAMo/Z@jPJXUpzL9@R6plKmncNm@ "Wolfram Language (Mathematica) – Try It Online"