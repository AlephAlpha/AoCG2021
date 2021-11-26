# [Pari/GP], 98 bytes

    f(n)=if(n,v=Vec(s=f(n-1));c=v[k=1];[if(c==d,k++,s=Str(k,s,c);c=d;k=1)|d<-v[2..#v]];Str(k,s,c),"1")

[Try it online!][TIO-kwbkbdff]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwbkbdff]: https://tio.run/##Rc3BCsMgEATQX5H0skvWUHsrdr@i0It4CNoUEaxo8NR/t@aUyzAwDyavJchP7n2DhBxGUuPX20Hl0aVC1I6biaysNmN2zJ7iPFPl514gUiV3EK8HwZ9/yGZuy3Jp1uoT0KQm7Nu3QBIsriTuJHIJaYfjFrH/AQ "Pari/GP – Try It Online"