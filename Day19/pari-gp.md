# [Pari/GP], 187 bytes

    a->m=vecmax;l=n=m([m(b)|b<-a]);forvec(v=[[i,k=(n+1)*n/2]|i<-r=[1..n]],u=v-r;if(![v[b[1]]>u[b[2]]|b<-a],d=Vec(sum(i=1,n,(x^v[i]-x^u[i])/(x-1)));if(#d<k,l=m(d);k=#d,#d-k||l=min(l,m(d)))));l

[Try it online!][TIO-kwrwrmpp]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrwrmpp]: https://tio.run/##JY7BboQwDER/JV0udjfZVdgjmM/oxfJKoZQqAlJEC6IS/04d1Zd5M5ZGM4clus/57A2dwTUTbR/vU9irkRJNwBO0eLS1C4JV/7XoEzZijnYgSFePr@leyhFrtxD72y2J2JU2t1SxhxfeuGUv0qyqpch/ke3oTWu@1wkieZss7M@No7j9uargHXbnETFXFF092FGHdFgNVHS26NxwHJrEBKPNeb5qPMM8j78QjGvMvMT0o3jJ5mJ6CIjWMHNpjRelhzW6Jkc@k4LqQ0Tw/AM "Pari/GP – Try It Online"