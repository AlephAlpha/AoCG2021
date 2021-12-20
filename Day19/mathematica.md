# [Wolfram Language (Mathematica)], 45 bytes

    1+Count[a=0;Sort@#,{b_,_}/;a==(a=b)]&@Sort@#&

[Try it online!][TIO-kxe03z1z]

A port of [@lonelyelk's Ruby answer](https://codegolf.stackexchange.com/a/239829/9288).

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kxe03z1z]: https://tio.run/##Tc1NCsIwEAXgfU8xUAiKIzXpj4USCXgBwWUpJS0Wu6iFElchZ4@JzsLVBzPvzSzaPB@LNvOo/QTS88N1fb9Mq@Wpua@bUSnaocfeZY2WcqflsO@Y@m2Yv21zyKZwvMDUpl0HDDKVgLVWIHcINkfhHCYQRjkCjaCKcgRBFlGBUEYLsopSN@zy/0xNN2rqhptn6nwt6VcRdc5/AA "Wolfram Language (Mathematica) – Try It Online"