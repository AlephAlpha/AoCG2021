# [Pari/GP], 94 bytes

    s->a=b=c=0;[if(a,a=0,if(d=="!",a=1,if(b,d==">"&&b=0,if(d=="<",b=1,d=="{"&&c++))))|d<-Vec(s)];c

[Try it online!][TIO-kwfrmr7q]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwfrmr7q]: https://tio.run/##ZY1BDsIgEEWvArMwbTpNdC1wDDdNF0Bb08RUIm4a5Ox1Rqs1kQD5/70hBHsb63NYBqGXWBurnfZ6f2zGobBo9R4pdFqDBGoHbg65G9jt3KYVoCPNMZHxVVXSenSqPvW@iGV79IsN4TIXUdRGhNs43SkCFxADTZQoGkgZUEBKKec1ZUz5C5E3uzdRGzErsQZ/zvqQE/7dHylf4PfepCQkDSPnSVGRhir9TJMM5j4qpaYrZZkVfdiWyxM "Pari/GP – Try It Online"