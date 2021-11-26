# [Wolfram Language (Mathematica)], 105 bytes

    SortBy[S=Subsets;Join@@Cases[Pick[s=S@#,#2Tr/@s,Tr@#]~S~#2,t_/;Sort@*Join@@t==Sort@#],0#|Times@@#&][[1]]&

[Try it online!][TIO-kwcxk0r5]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwcxk0r5]: https://tio.run/##jY29CsJAEIT7PMXCQgpZ0cTEH@Rk0c4qcOmOQ6JEPCQKubOQGF89RoMo2AizxbDfzBSZO@RF5swua/YgGnku3fKqpJCXrc2dna/P5sS8ymxuVWJ2R2WFZCQM03LAltKSUd/lHUNym8H8Gedel3FCvCxqGuItNUVumdHXSgVa@01SmpNTFWIN/QXsFaLW4AMze1BVVUAQEowIIoKYYEIwJZgRBMP2grp91eQB/AFG/4LxB@zYVuMvzX5Wu77Ru/Ubq5sH "Wolfram Language (Mathematica) – Try It Online"