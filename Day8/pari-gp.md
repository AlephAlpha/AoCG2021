# [Pari/GP], 155 bytes

    n->a=Map(Mat([p=i=0,d=1]));g=mapget;s=issquare;while(g(a,p)<n,p+=d*=I^(s(i)+s(-3+i+=4));mapput(a,p,sum(j=1,4,if(mapisdefined(a,q=p+I^j),g(a,q),0))));g(a,p)

[Try it online!][TIO-kwefbdnb]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwefbdnb]: https://tio.run/##JY1BjsIwDEWvErGyiSulDEigjtmz4AQIpEhNixFEbtNqxOlLwmy@/W3/Z/WjVL0uneElVkfPZ69w9hNclIUdtVxfEZueX177MDWJJaVh9mNo/u7yDNCDJ8XfSGq5XfPpBgkEbYLqx4rlbQ7nqM5TuaM0v@DBNW1JOshzSW3oJIY2bwdWe7o9kApyQHKI5fOXv2TE8w3RVEejo8Qpt6tiVqaDiEjmUpPZkDmQqfdkdi5Xl2VTZOf@rbvi8gE "Pari/GP – Try It Online"