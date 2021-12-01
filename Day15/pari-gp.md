# [Pari/GP], 105 bytes

    s->a=Map(Mat([p=c=0,1]));[if(while(c++;mapisdefined(a,p+=I^d),),,mapput(a,p,1))|d<-Vec(Vecsmall(s))%11];c

[Try it online!][TIO-kwnnu5b0]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwnnu5b0]: https://tio.run/##LUpLCsMgFLyKCAUfUajrRPddZNtNSED8tIIpElNLoXe32nSGgflFtXl2i8UhURKTSowqklHtZIpCizPlM0A/eUdedx8s0V3Xryr6ZKzzD2uIorETl8UABUrrEp976ygH@JiBXa0mVWlVIZAEcOJ87nWpv/AmCTGJ4uYfe7W4BYxce1E04bwcxBThReahqln5w3DgX@ScW5ihfAE "Pari/GP – Try It Online"