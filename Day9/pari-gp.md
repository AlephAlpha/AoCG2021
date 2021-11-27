# [Pari/GP], 65 bytes

    a->for(i=1,c=a[m=vecsort(-a,,1)[1]],a[(m+i-1)%#a+1]+=1);a[m]-=c;a

[Try it online!][TIO-kwhj3ldq]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwhj3ldq]: https://tio.run/##HczdCsIwDAXgVwkToWEpLP6gMrIXKbkIw0lBXalD8Olrt5vA4TsnyXL0j1QmkGJ@mObsojCNYuEl3/v4mfPivBExBlYlC@7VRs@431nL2gpjX6vqZeytWErPnzPwA2yfQIAJrgQpx/dSoVmpAaswOUNEghA6ggPBhaDTGo@0bk7bPRPcKqpi@QM "Pari/GP – Try It Online"

---

# [Pari/GP], 71 bytes

    a->c=a[m=vecsort(-a,,1)[1]];a+Vecrev((1/(1-x)%x^c-c/x)*x^m%(1-x^#a),#a)

[Try it online!][TIO-kwhjzfk0]

Longer but more interesting.

See the input as a polynomial, e.g. `[0, 2, 7, 0]` becomes $2x+7x^2$. Let $c\ x^{m-1}$ be its term with the largest coefficient (in this case, $c=7,m=3$). Then we subtract $c\ x^{m-1}$ from the polynomial, and then add $(x^m+x^{m+1}+\cdots+x^{m+c-1}) \bmod (x^n-1)$, where $n$ is the length of the input.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwhjzfk0]: https://tio.run/##HctdCsIwEATgqyyVQlY3tPEHFUmP4UtIYQltKVgbYinx9DH1YQdmPtZzGOXgUw86sWycZjPptXOfOSxCMpFCo6x98OHZudCtQqhKKBmxjK2Troq4j@1UblO7Y6R8ib1/fQWDbKCfgxhBgyK4EfgwvpcMxUYFcIZeMCISGFMTHAmuBLXN9UTbz/mfF4J7Rmsx/QA "Pari/GP – Try It Online"