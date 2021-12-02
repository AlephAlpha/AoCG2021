# [Pari/GP], 150 bytes

    (w,g)->p=vecprod;s=vecsum(w)/g;r=w;forperm(w,a,l=0;b=Vec(a);for(k=q=1,g,t=0;l=#[t+=c|c<-b=b[l+1..#b],t<s];q*=t==s);#b==#r&&p(b)<p(r)||#b<#r&&q&&r=b);r

[Try it online!][TIO-kwp4kauu]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwp4kauu]: https://tio.run/##hYzNasMwEIRfZYnAaJt1GjfpT5A3j9GL8EFSbROqNrLs1hT87q5MCIReCrMwO/MxwcRT3oa5AZ7lSC3mx8DftQvx/Kb6xfVfH3LE@1ZFHlVzjqGOKSBDnrfK8mvtpMGlkO/ccUEtDanwLPSwZje5MrdstV8Xm42wFQ1lX6nujgfmHpWwzCJmWZAWyyAjTpOw5ZJ0WRbZooqzCcH/SAP5EUI8fQ7JrpZnBc54LxsCg0igtS4IHgh2BHuCR4JngheCA0GxTVdUqaoW7l9sf8UuZNLTjQ5/hi5bu@viLVTh/As "Pari/GP – Try It Online"