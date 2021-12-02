# [Pari/GP], 105 bytes

    s->a=Map(Mat([p=c=0,1]));for(d=1,#s,while(c++;mapisdefined(a,p+=I^(Vecsmall(s)[d]%11)),);mapput(a,p,1));c

[Try it online!][TIO-kwoes1it]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwoes1it]: https://tio.run/##LYvNCsMgEIRfRSwFlxio50TvPeTaS0hA/GkFk0pMLX16q01nWZhvmAlyc@09ZIt4jq2QfJCBDHInY@CKXyibADr73IjmjJ4ifT@cN0Q1TbfI4KI21q1GE0lDw68zuRkVF@k9iTDq6cwYAIVaDa@9lmgJOpUL@w@JqBUobG7di8UVMLJlCRSNOM3HYYrwLFJfvlrxU3/oH6SUKkyQvw "Pari/GP – Try It Online"