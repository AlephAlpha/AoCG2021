# [Pari/GP], 69 bytes

    a->t=0;[[t=((t-i+=2)%8+3)*3\5+i|i<-Vec(Vecsmall(s))%15*2][#s]%8|s<-a]

[Try it online!][TIO-kwd4ji74]

Two observations:

-  The ASCII code of `DLUR` is `[68, 76, 85, 82]`, which becomes `[8, 1, 10, 7]` when modulus 15, which in turn becomes `[0, 1, 2, 3]` when modulus 4.
-  Going to the right, `[0, 1, 2, 3, 4, 5, 6, 7]` becomes `[1, 2, 3, 3, 4, 4, 5, 6]`, which is a part of OEIS sequence [A057355]: `a(n) = floor(3*n/5)`. There are many other sequences on OEIS, but this one seems to be the simplest. If your language has a one-byte built-in for the golden ratio, you may also use the sequence [A060143]: `a(n) = floor(n/φ)`.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwd4ji74]: https://tio.run/##JYpPC8IgGMa/ihgD321CbQSD5k7v0ZNgF/Mg0UJYIdNLsO9urh544Pf8CW71/BnyTER2fErieDEmCcYS943ooBqaHur@dm785kd@fdxZcXy5ZWERoDqd686aQ7TVsMWRO5tdCMuHOcInElb/TgXpHiiZmQNoiTFUS0lbQpVCxB2kVvhrdBFSW05lVGqvUEqt/ygRldKaWgv5Cw "Pari/GP – Try It Online"
[A057355]: https://oeis.org/A057355
[A060143]: https://oeis.org/A060143