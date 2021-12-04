# [Wolfram Language (Mathematica)], 156 bytes

    Min[Max@Total@IntegerDigits[2^#-2^(#-r),2,l+1]&/@Pick[{a,b}=#;s=Select[Range@Tr[r=Range[n=Max@#]]~Tuples~n,#r&&#[[b]]-b#[[a]]&],m=Max/@s,l=Min@m]]&

[Try it online!][TIO-kwrqi487]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwrqi487]: https://tio.run/##HY6xasMwGIRfRSAQDf2NsTIWFQ1dMgRC4u1HAdkojqisFFmBgFDWjO3L9LnyCK7c6b47juNGHc9m1NH2ej4RMW@tx62@yfYStZMbH81gwocdbJyQH2nFjy@0Civg4F4bxWq5s/0nJg1dFvT5/XibxME400fcaz8Y2QYM4h/Ri2WYKnVvr1/OTHcP9PnzGxijiJ1SVVdcQa0UUzAu7VpO4ET5JMcSzrtgfURKqndywjJEGKklSSlxaDKQtAaeF00NEL5A0XXOef4D "Wolfram Language (Mathematica) – Try It Online"