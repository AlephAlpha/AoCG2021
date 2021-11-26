# [Wolfram Language (Mathematica)], 70 bytes

    Array[c=Characters@#;""<>c[[Span@##]]==="nice"&,{1,1,1}Length@c,1,Or]&

[Try it online!][TIO-kwbigkzq]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwbigkzq]: https://tio.run/##RYvBCsIwEER/JSSQU0U8a0rEq6DiMeSwLlubQ6PEFGpLvz2mUXD2sDP7djqILXUQHUJqmEr7EOBtUB1aCICRwkuLLee7Go25PsFrIaxVSnHvkLispk2VZz6Sv8dWYw6nYGU6B@ejEWxVs0vvKJrG5J5lkq01m77linH/cCP2xcKi5T5mFZYDEhU4lI8bLsv5X7fwvxuIz@kD "Wolfram Language (Mathematica) – Try It Online"