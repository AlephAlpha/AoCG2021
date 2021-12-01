# [Pari/GP], 67 bytes

    (n,m)->c=0;forpart(x=n,forpart(y=n,lcm(Vec(concat(x,y)))-m||c=1));c

[Try it online!][TIO-kwiqvsx3]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwiqvsx3]: https://tio.run/##NYzNCoQgFIVf5dLKCwpp5QRhjzGbaCEyDYGVSIsJendHSVfnu/f8OO1X9nVhARXITjdko1H1sBzeaX@Sn9pp4SuyNRt5fwwxx250tOmFiGy7b6M44mCCds5eRAMbwfl1PyNW6ajAaGvJQkEjUpgmToHPEQQFkbShILM2SfvodwVEnYjLmO0Lda18vnlA5GIcaJPGSNNleJJpSZY6f80zhj8 "Pari/GP – Try It Online"