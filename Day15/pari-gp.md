# [Pari/GP], 100 bytes

    s->a=Map(Mat([p=c=0,1]));[mapput(a,while(c++;mapisdefined(a,p+=I^d),)+p,1)|d<-Vec(Vecsmall(s))%11];c

[Try it online!][TIO-kwrnyywl]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrnyywl]: https://tio.run/##LUzLCsMgEPwVEQqKCvWc6L2HXHsJCYiaVjBliaml0H@32nSGgXksC2YL4gZlQaokoY0aDJDB7GQEZdWZy4nSblwNwHMnhr/uIXpiGetqFZLzS3h4Vwdg6jI7yikDLunH9eLqLalKq4mRJEpPUk6dLfVTfJOEhEawhcdeLW4Bo6VdcTTiPB/EHOFZ576qWf1Df@Bf5JxbmGj5Ag "Pari/GP – Try It Online"