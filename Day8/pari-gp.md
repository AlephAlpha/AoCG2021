# [Pari/GP], 120 bytes

    s->i=#s;forvec(v=[[0,3]|k<-[1..#s]],prod(j=1,#s,prod(k=j,#s+a=0,a+=I^(Vecsmall(s)[k]%11+v[k])))&&i=min(i,#[1|a<-v,a]));i

[Try it online!][TIO-kwq48zfd]

Very slow. Iterate over all possible commands with the same length and find the one with minimal hamming distance.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwq48zfd]: https://tio.run/##LYxLCsMgAESvIkqDEg2RLqPue4FuxICkSTFfiUUo5O7WtF0M894sxtvdsadPA5ApMOUkCs2w7bHvcJRa1/RqjkkwzasKBWOo37cHHiWnKPx4kmPm0sqa2lLeWnzvu7DYecaB6MlcOC9jbkJIUTi5uBU7ijQ/rGCR2rw3Llnv5zcOgCngd7e@MsJTIBjyC6FAw7ZVKkYhIAVQCfWvr7YiqjPQkPQB "Pari/GP – Try It Online"