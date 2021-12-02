# [Wolfram Language (Mathematica)], 98 bytes

-5 bytes thanks to [@att](https://codegolf.stackexchange.com/users/81203/att).

    Ordering[i=1;s=I^ToCharacterCode@#~Mod~11;0Union@@Accumulate@Partition[s,i,i++,{i,1},0]-i&/@s,-1]&

[Try it online!][TIO-kwodmdnv]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwodmdnv]: https://tio.run/##NYyxCoMwGIRfJURwMaKZjSHFqUOpQzuFBIKm9YeqEGMW0Ve3Wuh9y303XG98Z3vjoTH7C5X73bXWwfCWUNJiKq/6MVadcabx1lVja0W03cZ2o7TInwOMgxCXppn7@WO8FbVxHvyxyokAgSQhCxC6klylEGdiIilV8V4f/15GKOXoJSOlUIwygRbMz2CCsA5/Tgtc88A0@/VDmNYscLzuXw "Wolfram Language (Mathematica) – Try It Online"