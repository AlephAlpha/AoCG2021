# [Pari/GP], 89 bytes

    s->vecsort([-#Set(Vec(Ser([I^c|c<-Vec(Vecsmall(s))%11])/(1-x^i),#s+1))|i<-[1..#s]],,1)[1]

[Try it online!][TIO-kwbgx7mz]

The easist eay to represent directions on a plane is using complex numbers, so we need to convert the input string to a list of `1, I, -1, -I`'s. The ASCII codes of `<^>v` is `[60, 94, 62, 118]`, which become `[5, 6, 7, 8]` when modulus 11. We only need to take the exponent with base `I`. This is `[I^c|c<-Vec(Vecsmall(s))%11]`. For example, the input `v>^>v<^<` would become `[1, -I, -1, -I, 1, I, -1, I]`.

After that, we need to split the list into chunks and take the cumsum. Unfortunately PARI/GP doesn't have many built-ins for list manipulation (unlike Mathematica). But we have polynomials and power series. `Ser` converts the list to a power series, so `[1, -I, -1, -I, 1, I, -1, I]` becomes `1 - I*x - x^2 - I*x^3 + x^4 + I*x^5 - x^6 + I*x^7 + O(x^8)`. And `/(1-x^i)` does exactly the job we want: split the list into chunks of length `i` and take the cumsum. For example, when `i = 3`, `/(1-x^3)` of the above sequence is `1 - I*x - x^2 + (1 - I)*x^3 + (1 - I)*x^4 + (-1 + I)*x^5 - I*x^6 + x^7 + O(x^8)`. `[[1, -I, -1], [1 - I, 1 - I, -1 + I], [-I, 1]]` is exactly the (column-wise) cumsum of `[[1, -I, -1], [-I, 1, I], [-1, I]]`.

Then we convert the power series back to a list with `Vec(...,#s+1)`. The length of the power series is `#s` (the length of the input). We add 1 to it, so that the resulting array includes an extra `0`, which represents the Santa's starting point.

The remaining steps are easy. `-#Set(...)` is the negation of the number of different elements in the list. We need to take the negation because we will sort it from the largest to the smallest.

`[...|i<-[1..#s]]` iterates the above computation with `i` running from `1` to the length of the input. `vecsort(...,,1)[1]` gives the index of the largest element.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwbgx7mz]: https://tio.run/##NYzBCgIhFEV/RRwCH@mEe3PfeqCN@GAQC2Eq8Q1SMP9uY9C9XDhnc/NckrrndmPnRsrWGOhVVuHUMMVVXGMQUyzCXTBswaju@@gxL4sggIPWHk5CqzcmkAMdNcCWjHJ6HAfyXkoNTvs257x8BDFlWS7pue7Iu3B26zeSOW57uGQc67/dqkVbDZof72IQTbXcQ/sC "Pari/GP – Try It Online"