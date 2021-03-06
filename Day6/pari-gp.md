# [Pari/GP], 49 bytes

    a->p=q=0;[[p,q]=[i-q,p+q]|i<-a];normlp([p,q,p+q])

[Try it online!][TIO-l0kobhug]

A port of [@tsh's answer]. Make sure to upvote that answer as well!

---

# [Pari/GP], 53 bytes

    a->vecmin([normlp(Pol(a)*x^i%(x^2-x+1),1)|i<-[0..2]])

[Try it online!][TIO-kwhac5bp]

If we see the city as the complex plane, then the instructions \$[a,b,c,\dots]\$ will end up at the point \$a+b\ x+c\ x^2+\cdots\$, where \$x={(-1)}^{1/3}=\frac{1}{2}+\frac{\sqrt{3}}{2}i\$ is a root of the equation \$x^2-x+1=0\$. So we can convert the input into a polynomial with variable \$x\$, and mod \$x^2-x+1\$. This gives the destination in the form \$a+b\ x\$.

`normlp(...,1)` is the usual taxicab distance: `normlp(a+b*x,1)=abs(a)+abs(b)`. If the destination lies in the first or the fourth sextant of the plane (i.e., \$a+b\ x\$ where \$a,b>0\$ or \$a,b<0\$), this already gives the correct result. In other cases we need to rotate the destination by 60° or 120°. 60° rotation is just multiplying by \$x\$, 120° is multiplying by \$x^2\$. We try all possible rotations and take the smallest taxicab distance.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-l0kobhug]: https://tio.run/##RY3BCsIwDIZfJezUYgKzepvdi4QccpkU5kyLF8F3r@0UBj/h@5LAb1oS3a0uEKvSbDHHcWI2zBI5UUY7ZfmkG6lM27M8VnP9uK99VbP17RRoBitpezUcugywOPUegVnaOCP0HDgihL@F3X4Jx1PDC8JVWskX "Pari/GP – Try It Online"
[TIO-kwhac5bp]: https://tio.run/##RY3hCsIgFIVf5TIIrqVjWj/XnqH/4kCiheDcRWI46N1NKxgcLt8H93DIRieelCe4ZiuG9XGfXUAdljh7wtvi0bJjGt0B06hEOknGJXu7XuiubZUxLFsiv6EFMQBFF14FmyoNTKXLOGhtypEcanbsOKi/qa/9ovangmcOlzryAQ "Pari/GP – Try It Online"
[@tsh's answer]: https://codegolf.stackexchange.com/a/238117/9288