# [Pari/GP], 178 bytes

    m->while(a=0*m;a[,1]=m[,1];while(a!=b=matrix(#a~,#a,i,j,m[i,j]&&[a[i,j],i>1&&a[i-1,j],j>1&&a[i,j-1],i<#a~&&a[i+1,j],j<#a&&a[i,j+1]]),a=b);m!=n=a+concat((m-a)[,^1],0*m[,1]),m=n);m

[Try it online!][TIO-l0ko4a26]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-l0ko4a26]: https://tio.run/##ZZDdasMwDIVfJU0h2IsM9u08535XewDjgVrWzaH2TEjpdrNXz5QfJxlDWOjok8TBCTsv3tNwKcwQRHP/8Nc3hkY@BI0WlDNhzHrpH8zJBOw7/8WO@ANHBA8tBEvZVZXFqQDfqKqiWqhRtYuCVihiT7Q46XqmpBdcK@c4oDlxHQ4mGqzPn/GMPWNBILfwSuvka/TDIZhIYwOmdP1mWIimSJ2PPSuf42PJ9awSw1yy8uXW78mFGIfCWgUK5Pqkln@0Ij3H0tEbzXy7ICeu1vnMtwuZrxccech4Cb0b31n4b2l/chf0jcMv "Pari/GP – Try It Online"