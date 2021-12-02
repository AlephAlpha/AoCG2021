# [Pari/GP], 125 bytes

    s->i=#s;forvec(v=[[0,3]|k<-[1..#s]],if(prod(j=1,#s,prod(k=j,#s+a=0,a+=I^(Vecsmall(s)[k]%11+v[k]))),i=min(i,#[1|a<-v,a-1])));i

[Try it online!][TIO-kwoe1pnc]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwoe1pnc]: https://tio.run/##LYxNCsMgGESvIoaCks8Q6TLqvhfoRhQkTYr5lViEQu5uk9DFMO8xMMFtnr1D7pHMkSkvi9j065a6liSpdQ13s4@CaV5VRTQGfE/Ctr7IIDkUES4e5XBw6WQNrpQPS55dG2c3TSRSPZob52U6mlIKXs5@IR4KzXcnWALH@Dk0PrsQpi@JiCkUNr98DsSnYNQfPxSQxtYqlZIQGBBWQv3rUiuSOoMNzT8 "Pari/GP – Try It Online"