# [Wolfram Language (Mathematica)] + [Combinatorica] package, 89 bytes

    <<Combinatorica`
    SortBy[Join@@Select[KSetPartitions@##,Equal@@Tr/@#&],0#+Times@@#&][[1]]&

[Try it online!][TIO-kwq1zfs9]

Using `KSetPartitions` from the built-in package *[Combinatorica]*.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[Combinatorica]: https://reference.wolfram.com/language/Combinatorica/guide/CombinatoricaPackage.html
[TIO-kwq1zfs9]: https://tio.run/##jY2xCsJAEET7fMXCQRpXNGrUgMqi2GgjxO448AwnHpgcnmshId8eI0EUbISZYmces7nms8k120zX9Wy2cvnRFpqdb4JDcJqnzvPyITfOFkSpuZiM5TY1vNOeLVtX3EgIXF/v@kK09z0SocK@6Oxtbm70uqSMlArrnbcFy1KICroLOEkhlIIQiCiAsiwjhAHCEGGEECNMEKYICULUbxxVTVVhAPAHOPoXjD9gyzYafyn5@druDd@r31hVPwE "Wolfram Language (Mathematica) – Try It Online"

---

# [Wolfram Language (Mathematica)], 105 bytes

    SortBy[S=Subsets;Join@@Cases[Pick[s=S@#,#2Tr/@s,Tr@#]~S~#2,t_/;Sort@*Join@@t==Sort@#],0#+Times@@#&][[1]]&

[Try it online!][TIO-kwq20f67]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwq20f67]: https://tio.run/##jY07C8JAEIT7/IqFhRS6onn4Qk4W7ayES3ccEiXiIVHInYWE@NdjNIgBG2G2GPabmTx1pyxPnTmk9RFELa@FW92VFPK2t5mzi83VXJjXqc2s2prDWVkhGQnDpBiypaRg1A/5wJDcbrh4xbnXZpwQb4uaRthPTJ5ZZvS1UoHWfr0tzMWpErGCwRKOClFr8IGZPSjLMiAICSKCmGBMMCWYEcwJglFzQdW8KvIA/gDjf8HxF2zZRpOO5j@rbV/0ae1iVf0E "Wolfram Language (Mathematica) – Try It Online"