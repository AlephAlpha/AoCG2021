# [Pari/GP], 184 bytes

    m->while(a=0*m;a[,1]=m[,1];while(a!=b=matrix(#a,#a~,i,j,m[i,j]&&[a[i,j],i>1&&a[i-1,j],j>1&&a[i,j-1],i<#a&&a[i+1,j],j<#a~&&a[i,j+1]]),a=b);m!=n=a+concat([(m-a)[,2..#a~],0*m[,1]]),m=n);m

[Try it online!][TIO-kwq99tlv]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwq99tlv]: https://tio.run/##VY9NbsMgEEav4tiSBfUQQZeheJ9VDoBYTKKmxQoUWa7abHJ1Z/zfCoHmzfs0GhK2Xnyk/pqZPoj659Pf3hka@RI0WlDOhOHVc39nziZg1/pfViAU@AAPDQRLrytLi2MBvlZlSbVQAzUzQSMUubcCR6wmSfiYdaWc44DmzHXYmWiwunzFC3bMsiCQW3jd7yntgJYblqJwMJHCPaZ0uzPMRJ2l1seO5cd4yLmeKDFcSpafvru/5kqOQ2atAgVyvVLLf6yIpzN39GYXv02Qo1drfvHbhMWvE@gz/RM "Pari/GP – Try It Online"