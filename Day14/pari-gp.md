# [Pari/GP], 64 bytes

    (n,m)->forpart(x=c=n,forpart(y=n,c*=lcm(Vec(concat(x,y)))-m));!c

[Try it online!][TIO-kwrn9sd3]

For explanation, please read (and upvote) [xnor's answer on Puzzle SE](https://puzzling.stackexchange.com/a/106278/10468).

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrn9sd3]: https://tio.run/##NYzBCsMgEER/ZZuTWxSqSWygmM/oJeQg0pSAMSI5NF9vlehp3uzOjNdhZV8fF1CROLohG5c9eB0O8lNGOVrdmdjclTUbeX8MMbszOmXoiYhsQ3zdTNTe25NoYCP4sLojYZNNA0ZbSxYKGpHCNHEKfE4gKIisLQVZtM06pH9fQTwycZmyQ6W@k9e1DIhSTANd1hRp@wJXMi/JWufPecb4Bw "Pari/GP – Try It Online"