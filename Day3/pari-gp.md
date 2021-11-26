# [Pari/GP], 91 bytes

    f(n)=if(n,v=Vec(s=f(n-1));c=k=0;[if(c==d,k++,k&&s=Str(k,s,c);c=d;k=1)|d<-v];Str(k,s,c),"1")

[Try it online!][TIO-kwgkfdxv]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwgkfdxv]: https://tio.run/##RY2xCsMgFEV/RTKE98gT4ljs/YpCltIhaFNEsKIhU//dminL4cK5cPJagv7k1jZKjNApB5a3o4q@tWG2DhGzfXbnAC9xmiSOY8VjLxSlijsv3kYY/vm7Pl72MjKYgdv2LZQU1CzqJiqXkHY6e8ztDw "Pari/GP – Try It Online"