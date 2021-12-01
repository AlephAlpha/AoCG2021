# [Wolfram Language (Mathematica)], 68 bytes

    Fold[StringDelete,#,{"!"~~_,"<"~~Shortest@__~~">"}]~StringCount~"{"&

[Try it online!][TIO-kwhkrwcf]

Mathematica has built-in regular expression support, but calling the function `RegularExpression` already takes 17 bytes.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhkrwcf]: https://tio.run/##ZY1BCoMwEEX3niIZwVVKL5AGoaXrgksRsTZWQQ1ouighuXo6aWsVCjOT/9@fMEOlWzlUuqsr35CDP6v@lmd66sb7SfZSSxYzAxScKxlwfLJWTVrOOi1L50CALdxn/ageo3ZgIPEX9DqPyU6QJo@LgiRkn0YGjAUWETDGWLtIy4xdMQsV0i/iKxILqgTb9PI3SPY3fyl9k@3cpBQZFYFda8zQUIEWr@NqAE85c85HhZpajjetfwE "Wolfram Language (Mathematica) – Try It Online"