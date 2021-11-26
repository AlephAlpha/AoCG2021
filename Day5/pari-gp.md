# [Pari/GP], 174 bytes

    (w,g)->r=w;forperm(w,u,forpart(p=#w,i=1;q=[t|s<-Vec(p),vecsum(t=Vec(u[i..(i+=s)-1]))*g==vecsum(w)];if(#q==#p,[if(#t<#r||(#t==#w&&vecprod(t)<vecprod(r)),r=t)|t<-q]),,[g,g]));r

[Try it online!][TIO-kwftps3x]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwftps3x]: https://tio.run/##VYzhasMwDIRfxTRQrFUuZB2FkaiPsT/GP0yWGEO6OopTM8i7Z/ZYxwYH@u50UrDslQvbIGiTCR2oC1NqhhuHnq85WbCw5SgDVQk91c1EOq5zq976TgbAe9/Ny1VGKn7R/niU/kAzqNoAPDmin0IC0/hBVhNRFVAXjG3F65pnjtJ@n4uBb@8yQvtABkCmCGts1WQAUTt0@W/Dmw1h/JRWqIsI7D9ixl0xO9HZcZQDCpuPhda6RpH1/K3zH70aFCdTKr/r00Mv/0sGti8 "Pari/GP – Try It Online"