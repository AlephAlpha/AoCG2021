# [Pari/GP], 66 bytes

    n->for(i=1,oo,if(sum(j=1,i,issquare((2*j-1)^2+8*i))>=n,return(i)))

[Try it online!][TIO-kwbm7xse]

House \$i\$ gets a present from elf \$j\$ \$\iff\$ \$n=\frac{k(j+k-1)}{2}\$ for some \$k \ge 0\$ \$\iff\$ \$k=\frac{\sqrt{(2j-1)^2+8i}-2j+1}{2}\$ for some \$k\$ \$\iff\$ \$(2j-1)^2+8i\$ is a square.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwbm7xse]: https://tio.run/##FctBDsIgEEDRq0y6GurQCInRDb1IUxPSFDONDhTahadH3P23@Mln1q9UA7gqegwxIztDMRIHLOcHtyYmLmU/fV4Rbb9po5728uhZqdEJ5fU4s2CTqj6l9xcF9Agpsxwtuz86CChKESxRFn/gZIbBXGeCyVgCcyewt7n9Pw "Pari/GP – Try It Online"