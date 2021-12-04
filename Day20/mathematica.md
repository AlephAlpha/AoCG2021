# [Wolfram Language (Mathematica)], 121 bytes

    f@_=1<0
    f@{y_,x___,z___,l_}/;Tr[1^{z}]==l:={x}~g~y
    x_~g~0=x=={}
    x_~g~y_:=Array[f@x[[;;#]]&&g[x~Drop~#,y-1]&,Tr[1^x],1,Or]

[Try it online!][TIO-kwrwdrqu]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwrwdrqu]: https://tio.run/##XU5NC4MwDL37KwqCpw6NnqbrcLD7dtitdEXGdIL7oHhoV@pfd7VF5gZN8l7y8tJ71d@u96pvL9U41iUnsEmCutSKY8k5x@8pddzExUlQOOu3YYR0OdHSDM2gAsltSYgkRBtPFM/JTohK0bqUlBZFyFgUNVQOe/F8DSFWK2ARdnaSYcAHwcajaB89DdFqi2o6LaC4DLROMEoMDpAGC/xz1IL1@huZa6ZOAFNYOVia2eKak8ii1GWYsV/zhrMtzOdgcddbpa6T@Svzf5ZgKUt/R//YmPED "Wolfram Language (Mathematica) – Try It Online"