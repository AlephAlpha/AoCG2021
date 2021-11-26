# [Pari/GP], 89 bytes

    s->vecsort([-#Set(Vec(Ser([I^c|c<-Vec(Vecsmall(s))%11])/(1-x^i),#s+1))|i<-[1..#s]],,1)[1]

[Try it online!][TIO-kwbgx7mz]

## Explanation

First we need to convert the input string to a list of `1, I, -1, -I`'s. The ASCII code of `<^>v` is `[60, 94, 62, 118]`, which become `[5, 6, 7, 8]` when modded 11. We only need to take the exponent with base `I`. This is `[I^c|c<-Vec(Vecsmall(s))%11]`.

After that, we need to split the list into chunks and take the cumsum. Unfortunately PARI/GP doesn't have many built-ins for list manipulation (unlike Mathematica). But we have polynomials and power series. `Ser` converts the list to a power series, and `/(1-x^i)` does exactly the job we want: split the list into chunks of length `i` and take the cumsum.

Then we convert the power series back to a list with `Vec(...,#s+1)`. The length of the power series is `#s` (the length of the input). We add 1 to it, so that the resulting array includes an extra `0`, which represents the Santa's starting point.

The remaining steps are easy. `-#Set(...)` is the negation of the number of different elements in the list. We need to take the negation because we will sort it from the largest to the smallest.

`[...|i<-[1..#s]]` iterates the above computation with `i` running from `1` to the length of the input. `vecsort(...,,1)[1]` gives the index of the largest element.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwbgx7mz]: https://tio.run/##NYzBCgIhFEV/RRwCH@mEe3PfeqCN@GAQC2Eq8Q1SMP9uY9C9XDhnc/NckrrndmPnRsrWGOhVVuHUMMVVXGMQUyzCXTBswaju@@gxL4sggIPWHk5CqzcmkAMdNcCWjHJ6HAfyXkoNTvs257x8BDFlWS7pue7Iu3B26zeSOW57uGQc67/dqkVbDZof72IQTbXcQ/sC "Pari/GP – Try It Online"