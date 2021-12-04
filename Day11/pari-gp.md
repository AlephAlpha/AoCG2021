# [Pari/GP], 90 bytes

    s->a=b=0;#[1|d<-Vec(s),if(a,a=0,if(d=="!",!a=1,if(b,d==">"&&b=0,if(d=="<",!b=1,d=="{"))))]

[Try it online!][TIO-kwrmgvvj]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrmgvvj]: https://tio.run/##ZY3NCoMwEIRfJdmCKKyg5yZ5jF7EQ@JPEYoN2oukeXa729oqNCTLzDcbxttpyK9@7YVe59xY7XRxPlXls1X5pWvSOcOhTy1aXbBotQYJKK0u2TpkYCBJ3J4ryh3lrANkdOrVen9b0lnkRvhpGB8kgQ2InioyFBWECCgghBDjpiKG@IPIl7MPUTsxG7EGD2/7yAr/5jeUb3Ccx1AaBq6hgIw0ZKmX9hgs3ayUGu@0j4ra6mx9AQ "Pari/GP – Try It Online"