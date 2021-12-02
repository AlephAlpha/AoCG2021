# [Pari/GP], 89 bytes

    f(n)=if(n,s=f(n-1);c=k=0;[if(c==d,k++,k&&s=Str(k,s,c);c=d;k=1)|d<-Vec(s)];Str(k,s,c),"1")

[Try it online!][TIO-kwootf0k]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwootf0k]: https://tio.run/##RY0xCsMwEAS/IlyYO3wCqwzKviKQJqQIUhzEgSIkl/67IldppthZmPKqyX5K7xtlRhqUhkHr2AcoVv8YYwCi6LKIznPDba@k0iScl@gVjo94tfd3oMZP/9cyuYn79q2UDcwq5iKm1JR3OmvM/Qc "Pari/GP – Try It Online"