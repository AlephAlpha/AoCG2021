# [Wolfram Language (Mathematica)], 174 bytes

    MorphologicalComponents[#,CornerNeighbors->1<0]//.m_:>Fold[If[{0,#2}~SubsetQ~Extract[#,#-{0,1}&/@Position@##],RotateLeft/@(d=#/.j_/;j!=#2->0)+#-d,#]&,m,Union@@m]/.k_/;k>0->1&

[Try it online!][TIO-kwghdyx3]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwghdyx3]: https://tio.run/##bY5hS8MwEIb/SiRQJqZNuo9qS2E4EFSmsk8ljGxN125NbqQRhJL99ZqBOFKE4z7cc8@9p4RtpBK23YmxRtn4CubUQAd7P@gWoE6gpbZ9ickCjJbmTbb7Zgumj/P0kXFKE7W5z5fQVeVzXQ6M4Lk7f35te2nfz0/f1oid9TKOPUpdRIsV9K1tQRcYc/IBVlj5ImtLi1mVYZocNvThcJPheZyz2zscVwTziCiy1henUJwmR79yzJl/IBpXptX@PopzVJeYcxQhWqBhGFKCfLGwM0fQwP4j6S/5qyu8kIkQOpModnXS8FroTKJCJ4hyzo0/ "Wolfram Language (Mathematica) – Try It Online"