# [Wolfram Language (Mathematica)], 49 bytes

    Max@Abs@{s=Fold[{#2-#[[2]],Tr@#}&,{0,0},#],Tr@s}&

[Try it online!][TIO-kwvfwx2h]

A port of [@tsh's answer]. Make sure to upvote that answer as well!

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwvfwx2h]: https://tio.run/##RYo9C8IwEED/ysFBpivG07USFzehg1vIED@KBVuhyVA47rfHWoXCG96D18f8fPQxd7dYWqjLOU7ueE1OUn16v@5ekCv0nkOgy@hQDYklq4RLJzWlGbshz59CdYDWYwhgYONARAlkS/BlVUvA/@KlfvA6zboj2KuWDw "Wolfram Language (Mathematica) – Try It Online"
[@tsh's answer]: https://codegolf.stackexchange.com/a/238117/9288