# [Wolfram Language (Mathematica)], 93 bytes

    Cases[{{1}}//.a:{{__},___}/;Max@a<#:>Reverse@Append[a,Accumulate@Last@a],b_/;b>=#,2][[1]]&

[Try it online!][TIO-kwyaozx2]

A port of [@Neil's answer].

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwyaozx2]: https://tio.run/##JcfRCoIwFIDhVzkgdHVqmyCUpky6LYhux5CjTRJSRGcEY9dd9qg9ghndfD9/S/ZmWrJNRXMN6Xyg0YzKOeE9YxuKnSsKj8UCS070lLQP4uxiHmYYjcz73nRXRZhX1dROd7JGHmm0kvTn/cKyYEmZpQGGWimh9Wo@D01nVQDrDGoVaA0rYBKcQAgRdghiixDxpXwh/BHx/3I/fwE "Wolfram Language (Mathematica) – Try It Online"
[@Neil's answer]: https://codegolf.stackexchange.com/a/238259/9288