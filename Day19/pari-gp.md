# [Pari/GP], 37 bytes

    a->v=0;1+#[1|t<-vecsort(a),v==v=t[1]]

[Try it online!][TIO-kxe05q5j]

A port of [@lonelyelk's Ruby answer](https://codegolf.stackexchange.com/a/239829/9288).

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxe05q5j]: https://tio.run/##TY3dCsIwDIVfJcybFVuw@3Og3YuUXBRxMhBXaikIvntNZgWvvpOcnBPvwqJuPs9gslNTMoeT3u@sfsezStfLcw2xdkImY5KJViNm5/39VTtQE/iwPMiGiocKZroUEqy1jQSNpFoJDbJg9dsMTM3Olx2TEj2zKxyYW5Kc9v9iLA1jSVLjsSQ29uVTx0QU@QM "Pari/GP – Try It Online"