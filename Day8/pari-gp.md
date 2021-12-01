# [Pari/GP], 131 bytes

    s->i=#s;forvec(v=[[0,3]|k<-[1..#s]],if(#(l=Vec(Ser([I^a|a<-v-Vec(Vecsmall(s))%11])/(1-x),#s+1))==#Set(l),i=min(i,#[1|a<-v,a-1])));i

[Try it online!][TIO-kwmyubrn]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwmyubrn]: https://tio.run/##LYzBCsMgEER/RZTCLtW00mPVe8@BXsSAlKRITSoxSAv59zQJPTx2Z2dnkh@DeKalI3rJwgTN8rV7j6V9QNHWnvnFzS8lrKwqlp3joQMGUd9Xv25HsLfGz16JIrbLSu59jJARD1I6PIEUH@QsHyWi1qxuJ4jIg@7DAIEzK/cw92J9RryGxacUv5CJMCSNYZjWlW6Ckm5r5cTSpjGmFKUoJ9Qo8x@7bFQxG9Th8gM "Pari/GP – Try It Online"