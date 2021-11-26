# [Pari/GP], 69 bytes

    a->t=0;[[t=((t-i+=2)%8+3)*3\5+i|i<-Vec(Vecsmall(s))%15*2][#s]%8|s<-a]

[Try it online!][TIO-kwd4ji74]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwd4ji74]: https://tio.run/##JYpPC8IgGMa/ihgD321CbQSD5k7v0ZNgF/Mg0UJYIdNLsO9urh544Pf8CW71/BnyTER2fErieDEmCcYS943ooBqaHur@dm785kd@fdxZcXy5ZWERoDqd686aQ7TVsMWRO5tdCMuHOcInElb/TgXpHiiZmQNoiTFUS0lbQpVCxB2kVvhrdBFSW05lVGqvUEqt/ygRldKaWgv5Cw "Pari/GP – Try It Online"