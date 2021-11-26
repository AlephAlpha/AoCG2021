# [Wolfram Language (Mathematica)], 68 bytes

    Array[c=Characters@#;""<>c[[Span@##]]==="nice"&,0{,,}+Tr[1^c],1,Or]&

[Try it online!][TIO-kwgjfvy3]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwgjfvy3]: https://tio.run/##TU5NSwMxEL3vrxiysGgb0V5TU1a8eWlhewsRxpDYIJuUJMXdlv72Nd0o@C7z5n0M02M66B6TVTjdLWB/Cg68MRB9r8F5G0f4xuCs@4ywuK@2xohudAkHxpTv5XpWdhgSYwm/9K/QpZAbb946xuLMs1EZ4NNLCDgKxV8PGFAlHWJbrwl53ighuiO6tq6l5JwTZ5UmDX26UHpd7oNYvStJV3QbZDPt8sUkanjYgBE5Dw08ttWldGgFJD9@VqfC8Yabc84obt6U1sUeSuhDzdO6vwtz5h8dNLlOPw "Wolfram Language (Mathematica) – Try It Online"