# [Wolfram Language (Mathematica)], 106 bytes

    Tr@Ordering[i=1;s=I^ToCharacterCode@#~Mod~11;-Length[{0}⋃##]&@@Accumulate@Partition[s,i,i++,1,0]&/@s,1]&

[Try it online!][TIO-kwbh4ge4]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwbh4ge4]: https://tio.run/##NY0xCoMwAEWvEgxkMaKZ1ZDiVGipg1tIIGjUQFWI0UV06dhb9iJWC/1veW/6nXKt7pQzpdprkO6FZQ9baWv6hpuUxGN6lcWQtcqq0mmbDZVmcLsP1UZIHNx037iWL9H6eb8gFIixS1lO3fRUTrNcWWecGXo@YoON72OCI4FCNmIi0J4fJ45DEFBQcygEQCBkYPHoOQ8DT85/zpqppHMik58fkUiZzNRb9y8 "Wolfram Language (Mathematica) – Try It Online"