# [Pari/GP], 65 bytes

    a->for(i=1,c=a[m=vecsort(-a,,1)[1]],a[(m+i-1)%#a+1]+=1);a[m]-=c;a

[Try it online!][TIO-kwep8klp]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwep8klp]: https://tio.run/##HYxdCsIwEISvMlSEhG6g6w8qJb1I2IelWAmoDbEInj6mfRlm@GYmaY7ukcoEX9QN05xN9Eyj1/Dy3/v4mfNinBKxDSxCGsyrjY7tfqctS@vZ9rUqzo@9Fk3p@TMKN2B7ggcTroSU43upoFlRg8motT208s0SQugIB8KF0EmNR1qXp03PhFuFIrb8AQ "Pari/GP – Try It Online"