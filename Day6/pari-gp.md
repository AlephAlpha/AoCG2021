# [Pari/GP], 53 bytes

    a->vecmin([normlp(Pol(a)*x^i%(x^2-x+1),1)|i<-[1..3]])

[Try it online!][TIO-kwbsnt4d]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwbsnt4d]: https://tio.run/##RY3hCsIgFIVf5TIIvKUjXT/XnqH/4kCiheDcRWI46N1NKxgcLt8H93DIRieelCe4ZiuG9XGfXWA6LHH2xG6LZxaPaXQHlkYl0kkil/h2vdCybTtjMFsivzELYgCKLrwKNlUamEoXOWhtypEcanY8c1B/U1/7Re1PBTsOlzryAQ "Pari/GP – Try It Online"