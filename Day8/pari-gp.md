# [Pari/GP], 140 bytes

    n->a=Map([p=i=0,r=d=j=1;1,0]);while(mapget(a,p)<n,p+=d*=I^(i++==j^2\4+1&&j++);mapput(a,p,r=sum(j=1,4,if(mapisdefined(a,q=p+I^j,&z),z,0))));r

[Try it online!][TIO-kwhhvdd2]

A port of my Mathematica answer.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwhhvdd2]: https://tio.run/##JY7RCsIwDEV/JfgwWptBOyYoM7774BdMB4Vt2rGVuCmiPz8zzcNNLrk5hP0Y0ivPLdAc04Onk2dVMgWyOFJNHbnCob3o4nULfaMGz9fmoTyy3kdkQ/WajpUKxhB1VXbOjUuSzhhdSJKfv6SApuegBIU5hnZhhKlu2hCbWvZ3YnOsOkw@Gj9otVQxznLdv1WE9AA8hviQcbWYFbQqao1QOoQMYYfgtggbK92KZIts7N/K3/MX "Pari/GP – Try It Online"