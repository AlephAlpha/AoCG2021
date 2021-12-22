# [Wolfram Language (Mathematica)], 65 bytes

    f@___=1<0
    f[0,x___,l_]:=l==Tr[1^{x}]
    f[a_,x__/;f@x,y__]:=f[a-1,y]

[Try it online!][TIO-kxgwc3hu]

A port of [@G B's answer](https://codegolf.stackexchange.com/a/239887/9288).

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kxgwc3hu]: https://tio.run/##XU29CsMgEN7zFEKgkyGemdLW4iN06BashFJpIOkQMiSIz25PRZoWPP3@/G7ql9dz6pfh0XtvpNZawJkVpmN0RUJHrY5iFOI2d3C3q1No9Tp49cnIlW46BFCrgG7KX@fhvXQlqS7EEClJqQ6kloW1jBLmaEEsIEgnUgRt@50mijwGIAzGAWmDTxRDCBGPN2ScvqXCXAt5HWRlvze1pWYelSYtzbE92Mf4r/WPnfMf "Wolfram Language (Mathematica) – Try It Online"