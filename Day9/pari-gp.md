# [Pari/GP], 87 bytes

    n->a=Mat(1);until(d=[b|b<-c,b>=n],s=0;a=Mat(Vecrev(concat(c=[s+=b|b<-a[,1]],a~))));d[1]

[Try it online!][TIO-kwyjj0qp]

A port of [@Neil's answer].

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwyjj0qp]: https://tio.run/##JYrBCoMwEER/ZfGU0A0kgtBi1z/otZeQQ4xaBFmD2kKh9NfTWOfwZh5M9MuoHjENQIlV4@nmN2Fk/eRtnERHtv20VxWwbYgdrqTr43Lvw9K/RJg5ZAtk1xP9r96icQ79V@bUnTUu@Rint2BQDcRl5C3PYpcCBsFSIliDUCJcEMwZodK5dUa5o9KHaifTDw "Pari/GP – Try It Online"
[@Neil's answer]: https://codegolf.stackexchange.com/a/238259/9288