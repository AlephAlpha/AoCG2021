# [Wolfram Language (Mathematica)], 79 bytes

    (a=#;Do[a[[Mod[m+i,Tr[1^a],1]]]++,{i,c=a[[m=Tr@Ordering[-a,1]]]}];a[[m]]-=c;a)&

[Try it online!][TIO-kwepu7ox]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwepu7ox]: https://tio.run/##JclNC4JAEIDhvzKwIIUjoRUUsuGhbn1cvA0TDKvmHjZh3Zv4203t9vI@TkJbOwnWyNSAnjaiVX7tSIgeXUUutlh6St/CmDJzHONg0eiZnS598fJV7e33Q4msPnK@EHOiTS7baHrWfaC79KG4mbYjBckFGlLMECEohNMcsCtgGDKEA0KKkI0Iw37N/zginJc9Tj8 "Wolfram Language (Mathematica) – Try It Online"