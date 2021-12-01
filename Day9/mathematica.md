# [Wolfram Language (Mathematica)], 100 bytes

    (Clear@a;a[a@_=p=i=0]=d=n=1;While[a@p<#,p+=d*=If[4i++<=n^2<4i,n++;I,1];a@p=a[p+I^j]~Sum~{j,4}];a@p)&

[Try it online!][TIO-kwhip1vs]

The spiral turns left at position 1, 2, 3, 5, 7, 10, ..., which is OEIS sequence [A033638]: `a(n) = floor((n^2)/4) + 1`.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhip1vs]: https://tio.run/##JYpBC4IwGIb/ygdCVFu0iUIxvxA6eQs6dBgzRipOdAyxk@hfX6suz8P78A56autBT@alfQPot9e@1mOuhZY6f6JDg0xhhRa5eLSmr0N2WUQdwWqPRSMTQ0iGtoyzxFBLiCgoVyKcUEtHirJT6/09rHNHk@XXdxt/G42dZASHCzQyUgo2cMxh5hRiCmcK/EQhZcEsIP4iZf/JFv8B "Wolfram Language (Mathematica) – Try It Online"
[A033638]: http://oeis.org/A033638