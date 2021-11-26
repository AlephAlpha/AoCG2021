# [Wolfram Language (Mathematica)], 106 bytes

    (Clear@a;a[p=a@_=i=0]=d=1;While[a@p<#,p+=d*=If[Or@@(1∣√{4i+1,4i++}),I,1];a@p=a[p+I^j]~Sum~{j,4}];a@p)&

[Try it online!][TIO-kwefczay]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwefczay]: https://tio.run/##JYzBCoJAFEV/5YEQmi@aEYXCXgy0clXQosUwxVBKIxoithJd@w1t@zN/xKbanMs9XG6pm3ta6sZc9ZQBTe6uSHUtdKxlRVpcyBBTdCMen@6mSKUW1cbByqfbnJJM7mshXD4O73F4taHxOVr4nYcJchXbMdkfPznnqj8@y77NMex@3ptNh9o8GunAYguZdJSCGSwFtBwhQFgj8BVCxGwyi@CLiP0r66YP "Wolfram Language (Mathematica) – Try It Online"