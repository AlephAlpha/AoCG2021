# [Pari/GP], 90 bytes

    s->a=b=0;#[1|d<-Vec(s),if(a,a=0,if(d=="!",!a=1,if(b,d==">"&&b=0,if(d=="<",!b=1,d=="{"))))]

[Try it online!][TIO-kwhl8m5e]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwhl8m5e]: https://tio.run/##ZY3LCoMwEEV/JZmCKIyg6yb5jG7EReKjCMUG7UbSfLudaW0VGpJw7zkJ4@005Fe/9kKvc26sdro4n6ry2ar80jXpnOHQpxatLji0WoMElFaXXB0yMJAkbveKvCPPOUBGq16t97clnUVuhJ@G8UERuIDoaUSGooIQAQWEEGLcUsQQfxB5s/sQtROzEWvwcLaPnPDv/kr5Bsd7l5KQNIxcQ4qKNFRpMr1ksHSzUmq8U5ZR0cA6W18 "Pari/GP – Try It Online"