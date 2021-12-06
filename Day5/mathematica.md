# [Wolfram Language (Mathematica)], 88 bytes

    <<Combinatorica`
    SortBy[Join@@Select[KSetPartitions@##,Equal@@Tr/@#&],1##&@@#+0#&][[1]]&

[Try it online!][TIO-kwtzlm17]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwtzlm17]: https://tio.run/##jY3NisJAEITveYqGhlxs2Yz/QnZpFC96EbK3YcBRIjtgMji2Bwl59jggorAXoerQVR/VlZW/srLiDrbr8nzpq72rrfgQg11y/C58kMVNr72rmYvyVB5Eb4pStjaIE@frCyPS6ny1J@bf8MWYGlKIKTP2snhorYxJu21wtegGsYX@Dxw1ojGQAjMn0DSNIhgQDAlGBGOCKcGMYE6gsmjVxqqlBOADcPQpOH6BDzZq8qb5v6@PveFz9R1ruzs "Wolfram Language (Mathematica) – Try It Online"