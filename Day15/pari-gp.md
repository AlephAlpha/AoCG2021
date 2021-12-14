# [Pari/GP], 89 bytes

    s->a=[p=c=0];[a=setunion(a,[while(c++;setsearch(a,p+=I^d),)+p])|d<-Vec(Vecsmall(s))%11];c

[Try it online!][TIO-kx5ku2bg]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx5ku2bg]: https://tio.run/##LYrBCsMgGINfRYSBosJ6bvW@F9hFLIi1q@C6n9o5Bnt3p@sSAslHwG5B3KDMSJYklJUapJNn02srk9@fa3isxHL9WkL0xDHWV5q83dxSMTB5GSfKKQNDP9Mgrt6RmnS3MZJE6anrTO@KBYhvkpBQCLaw7rXiNjCa24sjjfN4GHOER5WHmlbVT8OhP8g5t2Fo@QI "Pari/GP – Try It Online"