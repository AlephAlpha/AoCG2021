# [Wolfram Language (Mathematica)], 51 bytes

    !Outer[LCM,l=LCM@@@IntegerPartitions@#,l]~FreeQ~#2&

[Try it online!][TIO-kwiqnnr9]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwiqnnr9]: https://tio.run/##NYyxCsIwEIb3PsVJoFOEJmljl0pAEATFOpcOQVIttBVinEL76jGBZLn/4@6/b5bmrWZpxqd0AzRud/8Zpbvr6Yanxk8hxGUx6qV0K7UZzfhZvgLhqd/OWqnHhmjuWj0uprMIrbA/wtAh1PeQg3/NrCUYyIrBUgw0JMPAY7KQtb9XCWgRiHDfrRNVJffbDIKJRhOLhjKk77AqAi@Siqd/clhX9wc "Wolfram Language (Mathematica) – Try It Online"