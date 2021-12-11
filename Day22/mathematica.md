# [Wolfram Language (Mathematica)], 143 bytes

    Length[m=#~Mod~6&;##.E.E&@@#//.{a_ . 3 .b_/;a<6>b:>m[a+b+3],##&@@(a_ .#2.(o:#...).#2.b_/;a<6>b:>m[a+#].(##&@@m[-{o}]).m[b+#]&@@@{1|2,5|4})}]-2&

[Try it online!][TIO-kx1aoxb3]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kx1aoxb3]: https://tio.run/##jYzNC4JAEMXv/hUDA6K0jmbWoQ/x0q2g@7LE2vdhE8Lbuv7rZktGSVAwPObN/N5TsjwflCwvO9kcYdGsDtdTeeZqgfW62NcTd4ZIS1q6WYZhSFpugWAElG/DmZxP0nyaKi4H@WAkGGJLeQ8CY/KKKRKR/9h7MAryLKt4oAsjfFI8b6/tJdPDKmbjKjG@EUHsNpvb5VpyhCCFI0chwIUwc7SOGDzHMAd0zOA5nY2s/VD7Sqzta5caWvKLdtmx5b/oz4Y/e97aolfQmOYO "Wolfram Language (Mathematica) – Try It Online"