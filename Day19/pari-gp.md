# [Pari/GP], 196 bytes

    a->m=vecmax;;l=vector(k=(1+n=m([m(b)|b<-a]))*n/2,x,n);forvec(v=[[i,k]|i<-r=[1..n]],u=v-r;if(![v[b[1]]>u[b[2]]|b<-a],d=Vec(sum(i=1,n,(x^v[i]-x^u[i])/(x-1)));l[#d]=min(l[#d],m(d));k=min(k,#d)));l[k]

[Try it online!][TIO-kwrs0wuu]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrs0wuu]: https://tio.run/##JY7RbsIwDEV/JYMXe3NAKY8l/QxeLCOl6zpFbUKV0ahI/HuXwtM9Prq2PLnk9e@09squTjfB5p/v4Ja6Hje63xIMFsxXtAE4QIvP9qydIH7GY0ULRaz7WypNyJbZ0yBPf9bJsjkcogjNNutU@x4@OHPLRqSZS1Yi70PU2UtZ/psDeGsoEizXzF70cp1L4BEWbRCxHnnfiQ0@wosoQFfs8DID7bt3Z5DVTdP4AKd0o6bk473gbht2qgeHSIqZK1JGCp1IlU82ZTYqUPIkIrj@Aw "Pari/GP – Try It Online"