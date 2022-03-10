# [Pari/GP], 78 bytes

    n->for(i=!p=#a=Map(),n,iferr(mapdelete(a,p),e,mapput(a,p,1));p+=I^(#a*2\3));#a

[Try it online!][TIO-kyzh8s91]

A port of [@tsh's JavaScript answer](https://codegolf.stackexchange.com/a/239668/9288).

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kyzh8s91]: https://tio.run/##FYxBCgIxDAC/Uukl0SzoepTs3YM/WBYCplLQGEJ9f@0e5jBzGJeo08t7SdxtWso3oPLBOQs/xAHJqBaNgI/4U9/aFIQcSWkE/7Xd6IJ48xPfN8hynNfr0Cx9f1nidKY0DzyqNShgiNj/ "Pari/GP – Try It Online"