# [Pari/GP], 135 bytes

    (w,g)->p=vecprod;s=vecsum(r=w)/g;forperm(w,a,c=0;for(k=q=1,#a,c+=a[k];c%s||q++>2||b=Vec(a[1..k]));#b==#r&&p(b)<p(r)||#b<#r&&q>g&&r=b);r

[Try it online!][TIO-kwsnj93z]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwsnj93z]: https://tio.run/##jY3NasMwEIRfZYmpkfA6jfLTNijrx@hF6CCrtgl2GlluGwp6d1ciBEIvLczCzOzHrjP@WHZuboFmdsGOl5Wjr8Y6f36TU3LT54l5uvDHTrZn7xp/ipxBS6uUWU8jCcxiUZBRvZb2YQphLIpqHUJNr41lRonlstecy6wmynyeO1bzg2Oeh5DVh9SMVZfnnmou/WycG76ZgbIC54/vH9EuUliANcPAWgTDOYJSSiCsETYIW4QdwjPCC8IeQaziCB1XOnF/Ytv/YbsbdiWjnu60//Xvemtzu3gPaT7/AA "Pari/GP – Try It Online"