# [Wolfram Language (Mathematica)], 76 bytes

    Map[t=0;((t=⌊.6Mod[t-#,8]+1.8⌋+#)&/@Mod[2LetterNumber@#+2,22];t~Mod~8)&]

[Try it online!][TIO-kwhfkfwh]

A port of my PARI/GP answer.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhfkfwh]: https://tio.run/##JYnBCoIwGIBfZWwghlNrhxDE8LDjjBjsNHZYNcmDFfJ3En2A8il9kaX1nT6@r7Vwc62F5mJ9jQpf2aeGYpuHIRTz9E721eOqISY0M9EuyebpE5FNkJZrZsIBuO74as@uK0nEKGMmh3F5Y7YJjD91zR00QfEB1ZoYgwKUlqjvsRICU4Sl5JyvIpTkv6IWOB4o6pcp5Zq4EEr9VXAupVJ4GPwX "Wolfram Language (Mathematica) – Try It Online"