# [Wolfram Language (Mathematica)], 44 bytes

    1===Fold[{1-#,x#}[[StringLength@#2]]&,0,#]!&

[Try it online!][TIO-kwg0wi5g]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwg0wi5g]: https://tio.run/##y00syUjNTSzJTE78n6Zg@9/Q1tbWLT8nJbraUFdZp0K5Njo6uKQoMy/dJzUvvSTDQdkoNlZNx0BHOVZR7X8AUKIkWllB104hLVo5NlZBTUHfgau6ulaHS6FaKVgJSodDGX5KOgpKriDCLxxMusIkwILBEDIcSQFcQzCIwGMOXB02I9GMQbYBxUigUG3tfwA "Wolfram Language (Mathematica) – Try It Online"