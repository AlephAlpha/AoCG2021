# [Pari/GP], 181 bytes

    m->while(a=0*m;a[,1]=m[,1];while(a!=b=matrix(#a~,#a,i,j,m[i,j]&&[a[i,j],i>1&&a[i-1,j],j>1&&a[i,j-1],i<#a~&&a[i+1,j],j<#a&&a[i,j+1]]),a=b);m!=n=a+concat((m-a)[,2..#a],0*m[,1]),m=n);m

[Try it online!][TIO-kx43jhf1]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx43jhf1]: https://tio.run/##ZZBNbsMgEIWv4tiSBfUQQZeleN9VD4BYTKKmxQoushyl3fTq7vgH21U1As2bb3h6ImLnxXscLpkZgqjvH/76xtDIh6DRgnImjLde5gdzMgH7zn@xAn@gQPDQQLB0u7K0ODXga1WW1As1qmZR0AhF7JkeTrqaKekFV8o5DmhOXIeDaQ1W58/2jD1jQSC38Hg8FuiAoo2ROATT0uaAMV6/GWaizmLn257lL@1TzvWsIsPUsvz11u/JhRiHzFoFCuR6pJZ/tCI91zLRG018c5ATV@t@4ptD4quDowwJL6V367sI/yPtLXdFPzn8Ag "Pari/GP – Try It Online"