# [Wolfram Language (Mathematica)], 62 bytes

-3 bytes thanks to @att.

    _f=1<0
    f[0,x___,l_]:=l==Tr[1^{x}]
    f[a_,x__/;f@x,y__]:=f[a-1,y]

[Try it online!][TIO-ky2b04gd]

A port of [@G B's answer](https://codegolf.stackexchange.com/a/239887/9288).

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-ky2b04gd]: https://tio.run/##XU1BCsMgELznFUKgJ0Ncc0pbi0/oobdgJZRKA0kPIYcE8e12VaRpwdXZmXFm6pfXc@qX4dF7r42AMytMx@iqtaajVkcxCnGbO7jb1SmUeh20@mTkSjcdDMhVQDflr/PwXrqSVBdiiJSkVAdSy8JaRglztCAWEKQTVwRt@50mkjwaIAzaAdcGn0gGEyIeb8g4fUuBORZyHWRm35vSUjKPTJNKs20P9jb@K/1j5/wH "Wolfram Language (Mathematica) – Try It Online"