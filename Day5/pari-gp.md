# [Pari/GP], 154 bytes

    (w,g)->r=w;s=vecsum;p=vecprod;forperm(w,a,forpart(b=#w,i=1;e=[d|c<-Vec(b),s(d=Vec(a[i..(i+=c)-1]))*g==s(w)];#e-g||[#d==#r&&p(d)<p(r)||#d<#r&&r=d|d<-e]));r

[Try it online!][TIO-kwh9lgho]

First iterates over all the permutations of the input, and then iterates over the partitions of each permutation, and then filter out the correct partitions. Very slow. Timeout for most test cases.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwh9lgho]: https://tio.run/##VYvBasMwDEB/xdRQpM0uZB2F4aifsYvxwbWdYEhXo3QLA/97Fg82NniHJ@mpeM56LOsgaIVFjajPTIuZ6SOF@f1qSpPCt2iGG5fE1y3yqrnnO1xILipTZxLZWEOvX1OAC6oZIjX1Nh8OkB8poO4c4sNINMOCzsikx1qtjESS9/sCEfsCjLXK2LcNU6yx12n7Mrz6UqZP8EKfReH8dt9014adCH6aYFDCIyphre2U2Hj65vSHF6fE0bXk93z84fl/5HD9Ag "Pari/GP – Try It Online"