# [Wolfram Language (Mathematica)], 54 bytes

    1//.n_/;Tr@Boole[1∣Sqrt[Range[1,2n,2]^2+8n]]<#:>n+1&

[Try it online!][TIO-kwbmpkv4]

House \$i\$ gets a present from elf \$j\$ \$\iff\$ \$n=\frac{k(j+k-1)}{2}\$ for some \$k \ge 0\$ \$\iff\$ \$k=\frac{\sqrt{(2j-1)^2+8i}-2j+1}{2}\$ for some \$k\$ \$\iff\$ \$(2j-1)^2+8i\$ is a square.

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwbmpkv4]: https://tio.run/##y00syUjNTSzJTE78n6Zg@99QX18vL17fOqTIwSk/Pyc12vBRx@LgwqKS6KDEvHQgV8coT8coNs5I2yIvNtZG2couT9tQ7b9LfnRAUWZeSXSegq6dQlo0UE5HoTpPR8EQiAxqY/8DAA "Wolfram Language (Mathematica) – Try It Online"