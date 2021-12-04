# [Wolfram Language (Mathematica)], 68 bytes

    Fold[StringDelete,#,{"!"~~_,"<"~~Shortest@__~~">"}]~StringCount~"{"&

[Try it online!][TIO-kwrmhjlr]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwrmhjlr]: https://tio.run/##ZY3PCoJAEMbvPsU6gqeJXmBbhKJz4FFEzLYU1AXdDrHsvrrNVqYRzL/v980wXalr2ZW6qcrpynbTUbWXLNVD098OspVaYoQGQnCuQODU0loNWo46KQrnQIDN3Xt9r@69dmAgnk6kdRaxjWDXLMpzFrNtEhgwFjBgYIyxdh4tGrtg9OHdD@ILEjMqBa5yvvUj/tWvG77Iuv64ofDkXJFDIhQk6TctevCQI@e8V3SAnB7a6Qk "Wolfram Language (Mathematica) – Try It Online"