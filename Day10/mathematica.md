# [Wolfram Language (Mathematica)], 69 bytes

    Fold[StringDelete,#,{"!"~~_,"<"~~Shortest@___~~">"}]~StringCount~"{"&

[Try it online!][TIO-kwfqdx0s]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwfqdx0s]: https://tio.run/##ZY1BCoMwEEWvkozgKqUXSIPQ0nXBpUhIbVoFNaDpooTk6nZSbRUKM5P/358wnbK17pRtKjXdyWE6m/ZW5HZo@sdJt9pqljAHFEKQDDg@eW0Gq0ebSSlDAAG@DPP@0Tx7G8BBOl3Q2yIhO0HuRVKWJCX7jDhwHhgB55z3i/LM@R9ksWI2E74SsRAl2KaXj1Gxv/kN6Qds5xpSRFREdK0wQkMFWryMmxG89Mg57w1q6jke9NMb "Wolfram Language (Mathematica) – Try It Online"