# [Pari/GP], 110 bytes

    n->p=Pol(c=0);a=Map();for(i=1,n,if(mapisdefined(a,p),mapdelete(a,p);c--,mapput(a,p,1);c++);p+=x^c%(x^2-x+1));c

[Try it online!][TIO-kwrpmb5u]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrpmb5u]: https://tio.run/##HcxLCgMhEEXRrTgJVKFC21Op7CCQFTSInyB07MIYcPdGM3iDewaPXc36xSMJGkXfmZ7XCZ42tI4ejgFtuipkMqqonODtOH9CTLnEAE4xqikhnrHFf1qv9SL@ttXKTJESLUvqh79BP3bdpcHJYx0XQWJTYp/jmkuDBAURxw8 "Pari/GP – Try It Online"