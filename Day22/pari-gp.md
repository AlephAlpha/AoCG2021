# [Pari/GP], 162 bytes

    a->for(i=1,2*#p=Mod(Polrev(a)+y*x^#a,6),p=-if([[t=p%x^l+(3-s)*x^l--+(p\x^j+3)*x^j-=2|j<-[i..#p],x^(k=j-i)+1+1/(1-x)%x^k++==s=p%x^j\x^l=i-1]|i<-[2..#p]],t,p));#p-1

[Try it online!][TIO-l0hrdom8]

Based on [my Mathematica answer](https://codegolf.stackexchange.com/a/240011/9288).

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-l0hrdom8]: https://tio.run/##fY/RasMwDEV/xTQM7Frq4nTdy6b@wWDvngOGNcNuaEQahgv998xJGHSDDXHhyr5HSOz7gB88NoJGj/um62UgA9W6YHrp3uVr1/aHT@mVvqxTXXh4VMCEoZHWDsR3qW613OJZ5d8WUUt@S3XU26mPSNU1PqMNm03BDlItjxQxKG20uZcGk8r8UWui8zwqZralgMZdQ8aqGXMwACv1VDCa0TO3F@kF7gX34TRku5qalWjyjgqEtSXM5bKvYK7FlnCj6ekh2xstqXz6Ty3JHfzSH@l/iG@qXHLOqfEL "Pari/GP – Try It Online"