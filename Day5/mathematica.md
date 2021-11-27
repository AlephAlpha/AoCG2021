# [Wolfram Language (Mathematica)] + [Combinatorica] package, 91 bytes

    <<Combinatorica`
    f=SortBy[Join@@Select[KSetPartitions@##,Equal@@Tr/@#&],0#|Times@@#&][[1]]&

[Try it online!][TIO-kwh7orns]

Using `KSetPartitions` from the built-in package *[Combinatorica]*.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[Combinatorica]: https://reference.wolfram.com/language/Combinatorica/guide/CombinatoricaPackage.html
[TIO-kwh7orns]: https://tio.run/##jY3NCsIwEITvfYqFQE8rWv8LKoviRS9CvYWAsUQM2AbjepCaZ68VEQUvwsxhZz5mC81HU2i2ua7ryWThir0tNTvfBLvoMM2c5/lNrpwtiTJzMjnLdWZ4oz1btq68kBC4PF/1iWjr2yRihR1x39rCXOh5SZkoFdcbb0uWlRABWjM4SCGUghiIKIKqqhKELkIPoY8wQBghjBFShKTTOAlNFTAC@APs/wsOPuCLbTT8Uvrz9bXXe69@Y6F@AA "Wolfram Language (Mathematica) – Try It Online"

---

# [Wolfram Language (Mathematica)], 105 bytes

    SortBy[S=Subsets;Join@@Cases[Pick[s=S@#,#2Tr/@s,Tr@#]~S~#2,t_/;Sort@*Join@@t==Sort@#],0#|Times@@#&][[1]]&

[Try it online!][TIO-kwcxk0r5]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwcxk0r5]: https://tio.run/##jY29CsJAEIT7PMXCQgpZ0cTEH@Rk0c4qcOmOQ6JEPCQKubOQGF89RoMo2AizxbDfzBSZO@RF5swua/YgGnku3fKqpJCXrc2dna/P5sS8ymxuVWJ2R2WFZCQM03LAltKSUd/lHUNym8H8Gedel3FCvCxqGuItNUVumdHXSgVa@01SmpNTFWIN/QXsFaLW4AMze1BVVUAQEowIIoKYYEIwJZgRBMP2grp91eQB/AFG/4LxB@zYVuMvzX5Wu77Ru/Ubq5sH "Wolfram Language (Mathematica) – Try It Online"