# [Pari/GP], 59 bytes

    f=n->i=0;until(sum(j=1,i,issquare((2*j-1)^2+8*i))>=n,i++);i

[Try it online!][TIO-kwoomn78]

House \$i\$ gets a present from elf \$j\$ \$\iff\$ \$n=\frac{k(j+k-1)}{2}\$ for some \$k \ge 0\$ \$\iff\$ \$k=\frac{\sqrt{(2j-1)^2+8i}-2j+1}{2}\$ for some \$k\$ \$\iff\$ \$(2j-1)^2+8i\$ is a square.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwoomn78]: https://tio.run/##FcdRCoMwDADQqwS/Ek3FFsYGUi8iDoqsI@Jip/Zjp@@2v/dS2MU8U4ngS/RqBvFdn/WUFY/8wsVbFpbjeOewPxBdvRhLd9fcaiEavLI0DfVSQkrrBxXMAGkXPX@s/qkgohIxzJvO4cTRtq3tJobROgZ7ZXCXiah8AQ "Pari/GP – Try It Online"