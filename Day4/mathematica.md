# [Wolfram Language (Mathematica)], 32 bytes

    1//.n_/;Tr[1^Divisors@n]<#:>n+2&

[Try it online!][TIO-kwp1zk5z]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwp1zk5z]: https://tio.run/##y00syUjNTSzJTE78n6Zg@99QX18vL17fOqQo2jDOJbMsszi/qNghL9ZG2couT9tI7X9AUWZeSbSygq6dQlq0cmysgpqCvoOCV35mXnRQYl56arShQayOQrWhkY6CobmOgpFpbex/AA "Wolfram Language (Mathematica) – Try It Online"