# [Pari/GP], 71 bytes

    s->sum(i=1,#s,sum(j=1,(#s-i)\3,[Vec(s)[i+j*k]|k<-[0..3]]==Vec("nice")))

[Try it online!][TIO-kwfry85k]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwfry85k]: https://tio.run/##RYvBDsIgEER/hdALq9BoepV@hhfkUAk12yolxSa18d8R0MS57JudGd/NKG4@9kTGINqwPBjKI68CzzgkZFUQCJeGq7M1LIDC/bAb9Xs8CXWo60ZrKXNCHRpLASB23t9fLBDREj@jeyak2VDSpz1wor5dTqibcDNLwS4r/7ekkiVjrC3hWhpXkw@637bkf1ot1RA/ "Pari/GP – Try It Online"