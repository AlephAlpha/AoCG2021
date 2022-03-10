# [Wolfram Language (Mathematica)], 58 bytes

    (Clear@a;c=p=0;a@_=-1;Do[p+=I^⌊2/3(c+=a@p*=-1)⌋,#];c)&

[Try it online!][TIO-kyzhdlys]

A port of [@tsh's JavaScript answer](https://codegolf.stackexchange.com/a/239668/9288).

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kyzhdlys]: https://tio.run/##y00syUjNTSzJTE78n6Zg@1/DOSc1scgh0TrZtsDWwDrRId5W19DaJT@6QNvWM@5RT5eRvrFGsrZtokOBFlBG81FPt45yrHWyptp/oKKAosy8kui06LzYWB2F6jwdBQMdBSOD2tj/AA "Wolfram Language (Mathematica) – Try It Online"