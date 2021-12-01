# [Wolfram Language (Mathematica)], 44 bytes

    1===Fold[{1-#,x#}[[#2]]&,0,StringLength@#]!&

[Try it online!][TIO-kwhmzpfr]

A port of my PARI/GP answer. Instead of taking the derivative, we check if the factorial of the state is one.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhmzpfr]: https://tio.run/##y00syUjNTSzJTE78n6Zg@9/Q1tbWLT8nJbraUFdZp0K5Njpa2Sg2Vk3HQCe4pCgzL90nNS@9JMNBOVZR7X8AUKAkWllB104hLVo5NlZBTUHfgau6ulaHS6FaKVgJSodDGX5KOgpKriDCLxxMusIkwILBEDIcSQFcQzCIwGMOXB02I9GMQbYBxUigUG3tfwA "Wolfram Language (Mathematica) – Try It Online"