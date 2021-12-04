# [Wolfram Language (Mathematica)], 82 bytes

    (Clear@a;a[d=p=0]=1;(While[a[p+=#]>0d++];a@p=1)&/@(I^ToCharacterCode@#~Mod~11);d)&

[Try it online!][TIO-kwrpgw0t]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwrpgw0t]: https://tio.run/##LYhBCoMwFESv8jEgii2adUwIuOqi0EWhixDhYyIKWiWEbEq9elpr3zDwZmb0g53Rjx3GHnjMmsmik8hQGb7ySnPKsscwTlahWgtOtKhMUWiGcuU0T0uZXdr70gzosPPWNYuxkmzXxWyU5szkaby58ekVgbOAXhGtIYVSwisJ7ZHkBEkrQv3truJHffA/Qgj7eMcP "Wolfram Language (Mathematica) – Try It Online"