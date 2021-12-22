# [Wolfram Language (Mathematica)], 48 bytes

    AtomQ@ChineseRemainder[-Range@Tr[1^#],#/. 0->1]&

[Try it online!][TIO-kxhgm3f1]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kxhgm3f1]: https://tio.run/##RY3NCsIwEITvPsVCoKfUdvtDycFS8QW0eAsRgqY2h0aovZU@e1wTQViY4ZthdtLLaCa92Lv2Axz8cXlNl@40WmfepqfEuoeZZdpr9zTddZZ4Y4qzbA952qJK/Hm2bpEM0hYGyZSCBLJuB@vacMCSQx6uFkFKJCg2vgNYyRZEOFQUR5RHEeJfobzmQFs0gBgn8Vcn2kT3hWEIQ526RQyq8LbaNv8B "Wolfram Language (Mathematica) – Try It Online"