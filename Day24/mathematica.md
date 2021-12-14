# [Wolfram Language (Mathematica)], 75 bytes

    #=={}||NumberQ@*ChineseRemainder@@#&@Thread[i=0;If[#>0,{--i,#},Set@s]&/@#]&

[Try it online!][TIO-kx5vl87p]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kx5vl87p]: https://tio.run/##RY09C4MwEIZ3f8VBwKFENH5QpEQCnbqUfm3iYGvEDDpEO8X8dntNCoWDO5734b2xXQY5tot6tVsPfCOcG7uu5/f4lPoqdsdBTXKWN3TU1EktBAnFY9Cy7WrFk8Opr0mVUBNFihJL73IRcxPGgjThdtFqWmoCUQVoNQ2EEIsAjNlTYBmFxE1RupUxhKWlAYDBM0VCIcfYo8SvsvwrmBcUsAsLGPOV7Kcj3fvrC10Rczq6qQ9y9za3dvsA "Wolfram Language (Mathematica) – Try It Online"