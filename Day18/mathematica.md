# [Wolfram Language (Mathematica)], 89 bytes

    Max[s=Subsequences;Length/@Select[s[I^ToCharacterCode@#~Mod~69],FreeQ[Tr/@Rest@s@#,0]&]]&

[Try it online!][TIO-kwnplpwc]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwnplpwc]: https://tio.run/##XchBC4IwGIDhvzImeDLsFEQYg08GQWKlt7Fgzc8UUmmbEET@9WXRqdPL83bKNdgp12rla5L4TD2ETYrxYvE@Yq/RbvbYX10TswJvqJ2wYncuB2iUUdqhgaFCFkzZUE2rtYy4QTyK0sTshNYxy4JoKUMpQ38wbe9EQBZbUotAShKSmJEnBRoRmqfpNznknPM/AMBvzP7qs2Emffk3 "Wolfram Language (Mathematica) – Try It Online"