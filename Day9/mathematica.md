# [Wolfram Language (Mathematica)], 76 bytes

    Min@Cases[Nest[Reverse@Append[#,Accumulate@Last@#]&,{{1}},#],b_/;b>=#,2]&

[Try it online!][TIO-kwzq4q7q]

A port of [@Neil's answer].

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwzq4q7q]: https://tio.run/##JcdBC4IwGIDhv/LBYKcvnIJQhDLpWhFdx4hpnyg0ETe7yM4d@6n9hGV0eV5ea3xH1vi@MbGFIp76QR6MI6fO5Ly60pMmR7IaRxruimHVNLOdH8aTPBrnJdOf94vjsqQhINNY35J9XRYMM83jZeoHrxhsSmgV0xo4JBKWFCFD2CGkW4RcrBUr2Y9c/FeE@AU "Wolfram Language (Mathematica) – Try It Online"
[@Neil's answer]: https://codegolf.stackexchange.com/a/238259/9288