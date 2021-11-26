# [Wolfram Language (Mathematica)], 83 bytes

    Nest[Fold[ToString/@Insert[#2,#,2]&,#,Tr[1^#]<>Min@#&/@Split@Characters@#]&,"1",#]&

[Try it online!][TIO-kwbllfmi]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwbllfmi]: https://tio.run/##DYyxCsIwFAB/JTTQ6UFtN0EloAgOFqXdHk8INW0DbVKS5yR@e8xytxy3ap7NqtkOOo3imFoTGa9@eWPvOw7WTZW6uWgCo2xAQkNlZh@wfkk6nO7WKVlWqtsWy@o866AHNiEqmbuiLiA7XTw@8onx@bGGcURHRCC@DsQOxP5H6Q8 "Wolfram Language (Mathematica) – Try It Online"