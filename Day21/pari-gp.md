# [Pari/GP], 45 bytes

    (a,b,c)->sum(i=0,(#a-1)/b,a[b*i+1,c*i%#a~+1])

[Try it online!][TIO-kwunbran]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwunbran]: https://tio.run/##bZHNCsIwDMfve4qgCK1m2ExERpkvMnbIBkphSpl68OKrz206l@JoSf6/5hPquXHx2bcnyFrFWGKl4@PtcVEuM6iWHJPelsh5uXYbwmrtVkt@bajQLRNkkBskJEtoBtv5IuLkExhCaOSxIwfeGpFHo7UjyVyykudyxUQ71Yv@wbTpNaymv33nOgSbFVHE3tdPxRAfwTfueu/koocFVFzX6oTAWiPkORNCf4sOep2mApJQ70bdo9DyPU0HSETXBETWF/YSDj8YBnY/@gY "Pari/GP – Try It Online"