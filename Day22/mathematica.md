# [Wolfram Language (Mathematica)], 105 bytes

-7 bytes thanks to [@att].

    Count[Table[t=b.c,#+3].a.b&/@#/.List->Dot//.{(n:a|b|c).n_:>Dot[],(n:b|c.a.c).a:>a.n,(n:c.t.t).b:>b.n},a]&

[Try it online!][TIO-kxibkul7]

A port of [Anders Kaseorg's Perl answer](https://codegolf.stackexchange.com/a/240010/9288).

### A proof that the last rule in Anders Kaseorg's answer is not needed

As I said in the comment, the last rule is needed for minimizing the length of the word, but we only need to minimize the number of \$a\$s.

After applying the first 6 rules, there are only 6 possible cases between every two \$a\$s: \$c\$, \$bc\$, \$cbc\$, \$bcbc\$, \$cbcbc\$, \$bcbcbc\$. Since there is no \$ba\$ or \$caca\$, \$aca\$ can only appear at the beginning of the word.

Now let's apply the last rule \$cbcbcab\Rightarrow bcbcbca\$, and see what will happen before and after the \$a\$ in \$cbcbcab\$. Remember that the only way to decrease the number of \$a\$s is applying the first rule: \$aa\Rightarrow \varepsilon\$.

#### Before the \$a\$

If this is the first \$a\$ in the word, there isn't another \$a\$ for us to apply the first rule.

If it is not the first \$a\$, the only two possible cases between this \$a\$ and the previous \$a\$ are \$cbcbc\$ and \$bcbcbc\$, which will become \$bcbcbc\$ and \$cbcbc\$ respectively. So the number of \$a\$ will not decrease.

#### After the \$a\$

If this is the last \$a\$ in the word, there isn't another \$a\$ for us to apply the first rule.

If it is not the last \$a\$, there are 3 possible cases between this \$a\$ and the next \$a\$: \$bc\$, \$bcbc\$, \$bcbcbc\$, which will become \$c\$, \$cbc\$, \$cbcbc\$ respectively. In the last two cases, nothing else will change.

But the first case will produce a new \$caca\$: \$cbcbcabca\Rightarrow bcbcbcaca\$. Applying the rule \$caca\Rightarrow acac\$, this substring will become \$bcbcbacac\$, and further become \$bcbcabcac\$ (by applying \$ba\Rightarrow ab\$). Now the \$c\$ at the end of the substring might meet another \$c\$ and get eliminated. But there can't be another \$ca\$ right after the substring, so nothing else will change, and the number of \$a\$ won't decrease.

---

# [Wolfram Language (Mathematica)], 133 bytes

-10 bytes thanks to [@att].

    Length[##.E.E&@@#//.{a_ . 3 .b_/;a<6>b:>Mod[a+b+3,6],##&@@(a_ .#2.(o:#...).#2.b_/;a<6>b:>Dot@@Mod[-{-a-#,o,-b-#},6]&@@@1?2@*5?4)}]-2&

[Try it online!][TIO-kxh1cbs8]

First appends two dummy variable `E`'s to the list, then repeatedly replaces:

- \$a3b\Rightarrow\operatorname{mod}(a+b+3,6)\$
- \$a2\underbrace{1\cdots 1}_{n\ge0}2b\Rightarrow\operatorname{mod}(a+1,6)\underbrace{5\cdots 5}_{n}\operatorname{mod}(b+1,6)\$
- \$a4\underbrace{5\cdots 5}_{n\ge0}4b\Rightarrow\operatorname{mod}(a-1,6)\underbrace{1\cdots 1}_{n}\operatorname{mod}(b-1,6)\$

And then takes the length of the result and minus 2.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[@att]: https://codegolf.stackexchange.com/users/81203/att
[TIO-kxibkul7]: https://tio.run/##jY1PC4JAEMXvfYoFQZLWWft3ERShjh06dJMlZhclIVeo7aR@dlsXjQqhYHjwfjPvTYn6kpWoC4ldTqJuVz2UTk8orlmqIwGSOos1BwThssRhcCju2o/3lWYM6rkKsRGN9ECdwx6mnBpmiAkYimGMoHokQYP2QISxANVS5G53vBXmk0P8mOSpwzlxCUtmdR1QMkxLZ6ReUTLMaANrP9SuNtZ@65ha2ssJHbNbez@hPxv@7HlrC17Btu2e "Wolfram Language (Mathematica) – Try It Online"
[TIO-kxh1cbs8]: https://tio.run/##jYxLC4JAFIX3/YoLF8Rq5mqmLnrYLGpX0F5Ext6LFGJ2w/x20yGjIig4HO7hnu9cpTofrlJddrI@wrxeH8qTOqeItKKVIwR6HmmZA8EYqMi9qZzFSTFJNtU@lcNiOGZxxhCbptu2MCC3miAR9dv7BVhWSoiW4ppLjqxivOBoGrxhxWgRiEG0CPsm44FTb2@XUqUIPIFjilkGDniip7XP4CHDeqADBg910bfxze0rtPHTO2pkm1@8YyPb/@I/F/7ceVnzn6Ax9R0 "Wolfram Language (Mathematica) – Try It Online"