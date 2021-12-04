# [Pari/GP], 138 bytes

    (w,g)->p=vecprod;s=vecsum(r=w)/g;forperm(w,a,c=0;for(k=q=1,#a,c+=a[k];c%s||q++>g||b=Vec(a[k+1..#a]));#b==#r&&p(b)<p(r)||#b<#r&&q>g&&r=b);r

[Try it online!][TIO-kwrnuut8]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrnuut8]: https://tio.run/##jY3RasJAEEV/ZTA07JKJdavWSpx8Rl/CPmzWJIhRJ5u2Uth/T3cRQfrSwgzce@dwh4075B1PLdAkrtjJvGT6aiy7y74Yoxo/T8LRVT53RXtx3LhT4AxaWkQvjjSQwiQEGZnqqAv7NHo/ZFnZeV/Te2NFiDM1nydGS1kkNVHi0pRFLXcsnPQ@qXcxGcouTR3VsnCTYe6/hYG8BHaH80eQs2hmYE3fixbBSIlQVZVCeEFYIqwQ1ggbhDeELYJahFU6nHTk/sRW/8PWd@xGhnl9mO2vf7eu5b3xEdJy@gE "Pari/GP – Try It Online"