# [Pari/GP], 138 bytes

    n->a=Map([p=i=0,r=d=j=1;1,0]);while(mapget(a,p)<n,mapput(a,p+=d*=I^(i++==j^2\4+1&&j++),r=sum(j=1,4,if(mapisdefined(a,q=p+I^j,&z),z,0))));r

[Try it online!][TIO-kwq5dpmt]

The spiral turns left at position 1, 2, 3, 5, 7, 10, ..., which is OEIS sequence [A033638]: `a(n) = floor((n^2)/4) + 1`.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwq5dpmt]: https://tio.run/##JY7BDoIwDIZfpfFANleSjWCiwXr34BOgJEsAHYGlgsboy2PRHv72O/TLz34M6ZXnFmiO6cHTybMqmQJZHKmmjlzh0F508bqFvlGD52vzUB5Z7yMK8fNHhuo1HSsVjCHqquycG5cknTFaNNNzUCLCHEO7GMJUN22ITS2fd2JzrDpMPho/aLVMMc7i7d8qQnoAHkN8yLlaYAWtilojlA4hQ9ghuC3Cxsq2EtkSG/tHaT1/AQ "Pari/GP – Try It Online"
[A033638]: http://oeis.org/A033638