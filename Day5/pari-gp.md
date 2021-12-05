# [Pari/GP], 144 bytes

    (w,g)->p=vecprod;s=vecsum(r=w)/g;forperm(vecsort(w),a,c=0;for(k=q=1,#a,c+=a[k];c%s||q++>2||b=Vec(a[1..k]));#b==#r&&p(b)<p(r)||#b<#r&&q>g&&r=b);r

[Try it online!][TIO-kwsusjt6]

TIL: the `forperm` built-in only works for sorted lists. Thanks [@tsh](https://codegolf.stackexchange.com/users/44718/tsh) for providing a new testcase.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwsusjt6]: https://tio.run/##jY3daoNAEIVfZYhUdnBMY37aBjM@Rm/Ei9WqBE1dx7RS2He3bkNKCZQWzsDMOR9njJZjWJupAp7USDWGieH3sjDSvcSD24a3kxIe8b6Oq05MKSfl3E7OakTSVPDKBarhniPyZiNgnTZZXNwN1vZBkKytzfm5LJROo@WyyRBjL2f2xPeNyvFglKC1Xn5wTp/Uvi@cYyyTNqb9UBrCBIwcX8/zunDHAgrdtqoi0IgEaZpGBGuCDcGWYEfwSPBEsCeIVvNE2RxljvsT2/4P212xCznr4Yf2N/8uXZtr4y30na1/0xea4fQJ "Pari/GP – Try It Online"