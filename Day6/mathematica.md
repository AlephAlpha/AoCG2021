# [Wolfram Language (Mathematica)], 55 bytes

    Min[Tr/@Abs@Fold[s=ReIm@{1-I,1,I};#.Most@s+#2s&,0s,#]]&

[Try it online!][TIO-kwhe7kjn]

If we use a coordinate system with basis \$(0,1)\$ and \$(\frac{1}{2},\frac{\sqrt{3}}{2})\$ (in the Cartesian coordinate system), then 60° rotation is just multiplying by the matrix \$\begin{pmatrix}1 & -1\\1 & 0\end{pmatrix}\$.

In each step, instead of turning the taxi and going forward in the new direction, we rotate the whole city and moving in a fixed direction. We choose three fixed directions, represented by \$(1,-1), (1,0), (0,1)\$ in the new coordinate system. One of the threes destination falls into the first or the third quadrant (or should I call it sextant?). Then we can take the taxicab distance as usual.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwhe7kjn]: https://tio.run/##y00syUjNTSzJTE78n6Zg@983My86pEjfwTGp2MEtPyclutg2KNUz16HaUNdTx1DHs9ZaWc83v7jEoVhb2ahYTcegWEc5Nlbtf0BRZl5JdLVyrYKunUJaNFBMQU1B30GhurpWR6HaUEcBhBBMAx0FIyjPCMyDICOEIiDTWEfBpLb2PwA "Wolfram Language (Mathematica) – Try It Online"