# [Pari/GP], 140 bytes

    (w,g)->p=vecprod;s=vecsum(r=w)/g;forperm(w,a,c=q=0;for(k=1,#a,c+=a[k];c%s||q++==g||b=Vec(a[k+1..#a]));#b==#r&&p(b)<p(r)||#b<#r&&q==g&&r=b);r

[Try it online!][TIO-kwq169s7]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwq169s7]: https://tio.run/##jY3RasMwDEV/RdQs2ETp6rXdVlz1M/YS/GC7SShNV8fZVgb@98ymFMpeNpDg6uroyptwqDo/tUATv2Anqp2nr8b5cN6rMavx88QDXcRjp9pz8E04Jc6go4EW2eFHksiSUZKpj1q5hzHGoSyJuhgtvTWOJ7@U8zkzWgjFLBELReG5FVvPg4iR2W12hnRSFIGsUGEy3vff3EC1Ax8O7x9JzvIwA2f6nrcIRgiEuq4lwhPCEmGFsEZ4QXhF2CDIRWqp00pn7k9s9T9sfcOuZKrnu9r8@nfNWt4S7yEtph8 "Pari/GP – Try It Online"