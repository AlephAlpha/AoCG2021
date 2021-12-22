# [Pari/GP], 151 bytes

    a->c=concat;[p,q]=[c([[[i,j]|j<-[1..#a],a[i,j]==t]|i<-[1..#a~]])|t<-[1,2]];vecmin([#[1|y<-q,![1|z<-c(p,q),!matdet(Mat([u=x-z,v=z-y]~))&&u*v~>0]]|x<-p])

[Try it online!][TIO-kxid1gb9]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxid1gb9]: https://tio.run/##bY7RasMwDEV/xW2h2EMucV8d5w/2BUYPwmtHypq5xQ1NMPn1TPY22MMQQkdXl4si3Xv9HtezcCvpLrjwOQRK1ke4ofNBeu97uGC@tNqbw2FHCFQV5xLm/lddEFVOZYMjoh1P4doP0u@8yVOrb7BhmFsdJOcq2FwpvZ2SfKUk/cM99Qyjm/WEi1L7/eNlXLoGMT9bHVGtFOPHJEnoTsR7PyTGbVm24ixJKRC@5BiGmmeg/FDkI9Sy/0@DbGkKQGO5uYwtG7ctIXwrlh@sx6ayqfa/xBf7HVVy@ecv "Pari/GP – Try It Online"