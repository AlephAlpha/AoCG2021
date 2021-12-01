# [Wolfram Language (Mathematica)], 78 bytes

    (a=#;a[[Mod[m+i,Tr[1^a],1]]]++~Do~{i,c=a[[m=Tr@Ordering[-a,1]]]};a[[m]]-=c;a)&

[Try it online!][TIO-kwhjnbrd]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhjnbrd]: https://tio.run/##HYvLCsIwEEV/ZSBQlE6x9YFKiXShOx8bd0OEIW1tFrFQuwvpr8fYzeHAPdfy2DWWR6M5tCDDgqUomejW12RTg8@BihcrLJRSaTqd@8kZ1DIWVj6H6jHUzWA@b8p4Tvz/a5XKpC55mYR78x3pyhEX3fUkIDtBSyKWkCAIhEMUWFXgXI6wRtgj5B7BbRAKhO3MHcIxjt6HHw "Wolfram Language (Mathematica) – Try It Online"