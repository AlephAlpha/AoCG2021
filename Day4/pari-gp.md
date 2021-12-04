# [Pari/GP], 32 bytes

    n->i=1;while(numdiv(i)<n,i+=2);i

[Try it online!][TIO-kwrf99ce]

House \$i\$ gets a present from elf \$j\$ \$\iff\$ \$i=\frac{k(j+k-1)}{2}\$ for some \$k \ge 0\$ \$\iff\$ \$k=\frac{\sqrt{(2j-1)^2+8i}-2j+1}{2}\$ for some \$k\$ \$\iff\$ \$(2j-1)^2+8i=l^2\$ for some \$l\$ \$\iff\$ \$8i=(l+2j-1)(l-2j+1)\$ for some \$l\$ \$\iff\$ \$m-8i/m=4j-2\$ for some divisor \$m\$ of \$i\$.

So house \$i\$ gets \$n\$ presents \$\iff\$ \$8i\$ has \$n\$ divisors \$d\$ such that \$d\equiv 2 \pmod{4}\$ \$\iff\$ \$i\$ has \$n\$ odd divisors.

But \$i\$ and \$2i\$ has exactly the same number of odd divisors. So we only need to consider the odd numbers, whose divisors are all odd.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrf99ce]: https://tio.run/##FcdBDoJADADArzSc2tAldhPjAZePEA4bBG2CtSEo4fWr3mY8rxruXmZIxUKnSdr9ocuE9n7e9INKV2OtU6RWS3ZfDjQIHfiqtv1Y/VPBjEbEML5szBv20jRyGhh6iQxyYYjngah8AQ "Pari/GP – Try It Online"