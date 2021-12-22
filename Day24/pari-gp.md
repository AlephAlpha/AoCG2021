# [Pari/GP], 48 bytes

    a->i=0;iferr(chinese([Mod(i--,b+!b)|b<-a]),e,x)'

[Try it online!][TIO-kxh9susa]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxh9susa]: https://tio.run/##NY3bCsIwDIZfJe7GFlNod2AU3d7AJxi96LTTgsxSvVDw3WtaEUIO3/8nCTZ6cQlpgSFZMfpB7v3iYmSnq1/dw7HpeD8zLwTOu83MP/NBWMPR4Ytvkw3h9mYWxAgh@vVJbZWHChZmOUeYph5BNQiyRKdLaRRBbUimpqYZoSUxA5mT1n@RlA6BbtCiUr9TqhiJ9blmUNZVsZKvzrgtj1pjePoC "Pari/GP – Try It Online"