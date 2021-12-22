# [Pari/GP], 179 bytes

    f(a)=p=Mod(Polrev(a)+y*x^#a,6);while(p!=q=g(g(p)),p=q);#p-1
    g(p)=-if([[t=p%x^l+(3-s)*x^l--+(p\x^j+3)*x^j-=2|j<-[i..#p],x^(k=j-i)+1+1/(1-x)%x^k++==s=p%x^j\x^l=i-1]|i<-[2..#p]],t,p)

[Try it online!][TIO-kx1gyrom]

Based on my Mathematica answer.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx1gyrom]: https://tio.run/##fY/RSsNAEEXf/YrYIMy4M7Wbqi91/APB97iBgG3cdLHTNGgK/fe4SRBKQRku3DvcMzBaNp4r7fsNlCgqL7t3eN2FZv0VsznedkVa0iOuvj98WINey14qqEARSWWPq1TZXg1Z2G8gz1vRm64IBpZ8wEgHZgP61hW1WQ65ZslO9RPnfj5P1VFXwFZq9missXdgucPIb40ROYyn6sgG8WzdyUcsGzFHLSn2pWo4Qpnwc6KN/2yjnQ1hlgzfICV5vqBxXPQZjTPZBZ1pWN1He6apZelCU/OBLvRH@x/il1pMPeew/wE "Pari/GP – Try It Online"