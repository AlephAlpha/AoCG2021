# [Wolfram Language (Mathematica)], 83 bytes

    Nest[Fold[ToString/@Insert[#2,#,2]&,#,Tr[1^#]<>Min@#&/@Split@Characters@#]&,"1",#]&

[Try it online!][TIO-kwgkv5t6]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwgkv5t6]: https://tio.run/##JYzLCsIwFET3/YqLgaIlUHVnfRBQBAUf0O5ChFATDdgbSSIi4rfHoJuZOXCYToar6mQwrYz9ApqHQ7Bag7edArTGv@ApHRq8eCgG2UFrXgeXcGsNVpX/bTHNMg3zuFc@8LW9nXlj/1bJNuiVC5yMKaFjkadsHB@diJgtdgYZyUtW328msOVVOtkG5TwjyeuNejR1XFl@TE@Ba45CUHgjhSGFyUfELw "Wolfram Language (Mathematica) – Try It Online"