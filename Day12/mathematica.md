# [Wolfram Language (Mathematica)], 109 bytes

    #//.x_:>(x-#+RotateLeft/@#&)@ImageData@SelectComponents[Image@x,#BoundingBox[[1,1]]>0&,CornerNeighbors->1<0]&

[Try it online!][TIO-kwhvk914]

Repeatedly select the components whose bounding box's `x_min` is greater than 0, and move these components 1 unit to the left.

The `SelectComponents` function has a bug: when it takes an array instead of an image as input, the `CornerNeighbors` option does not work. So we have to convert the input into an image.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhvk914]: https://tio.run/##fY1vS8MwEIff71OEBopiZpO3Q0vYRBj4D@e7NEicaVcwF8luECj97LUqTBtEOO7gnnvu5wzurDPYbs1Qk8uBFsV5fF6UJ3FOzx49GrQ3tsZC0vxUrp1p7JVBIzf2zW5x5d27Bwu4V19IRkaX/gCvLTRLH5USTGhd8pytfAAb7mzb7F582M9LccF1PjyEFlBla1hUUEHGyJPf4Lhr1K0ZZ7z2wSmqNSNZBfcH/O@s/jzUmuSkkLOu6wQjY/Fp5z2bEdLxv5g4smP94G@WSKmXRPLfnpj@TL0kMvUmkX3fDx8 "Wolfram Language (Mathematica) – Try It Online"