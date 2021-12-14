# [Pari/GP], 53 bytes

    a->iferr(chinese([Mod(-i,b)|i<-[1..#a],b=a[i]]),e,x)'

[Try it online!][TIO-kx61t6jg]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx61t6jg]: https://tio.run/##NY7dCsIwDIVfJcwLW0jHuh9Gwe0NfILSi047Lcgs1QsF372mFSE0yXdO0gQbvbiEtMKUrJj96mJkp6vf3MMxfbyfmfC48I8/CC3remcNLpPV3hiODl98n2wItzezIGYI0W9PKqvcVLAyyzmC1iOC7BCaEoMqqZMElSGZipZ6hJ7EDJr8KPUXSRkQaAcNSvlbJYuR2JhzBmVcFiv52oz78lFPp6Yv "Pari/GP – Try It Online"