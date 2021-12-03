# [Pari/GP], 118 bytes

    s->i=#s;forvec(v=[[0,3]|k<-l=Vec(Vecsmall(s))%11],#Set(Vec(Ser([I^c|c<-l+v])/(1-x),m=#l+1))-m||i=min(i,#[1|a<-v,a]));i

[Try it online!][TIO-kwqgqrgx]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwqgqrgx]: https://tio.run/##LY3BCsMgGINfRSwDf6pssmPV@86FXcSClHbIbCe1yAa@u7Njh5B8IZBgN8ceocxIlsiUk03s5teWppEkqfWFXk1@CublvTZVcbHekwhw4tzQpp/2oyX9tBF9G8Y81m2bDJwJZ2@gi2x8ywHYkrOTi1uJo43m2QqWqDUAnSs2BP8hETGFwubWvUZ8AEbzcUSRxsOgVEpCYIqwEupvPxxEUoewgfIF "Pari/GP – Try It Online"