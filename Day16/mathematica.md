# [Wolfram Language (Mathematica)], 373 bytes

    (Clear@A;P=ToExpression@StringSplit@#;S=A/@{0,1};(#@_=0;#@p=#[[1]];#@i_?NumberQ:=i;#@C={};#@N=1)&/@S;While[0<#@N<=Length@P&/@And@@S&&(#@C!={}||P[[#@N,1]]=!=rcv&/@Or@@S),(P[[#@N]]/.{i_,x_,y_:0}:>Switch[Y=#@y;i,set,#@x=Y,add,#@x+=Y,mul,#@x*=Y,mod,#@x=#@x~Mod~Y,jgz,#@x>0&&(#@N+=Y-1),snd,(1-#&/@#)@C~AppendTo~#@x,_,If[#@C!={},{{#@x},#@C}=#@C~TakeDrop~1,#[N]--]];#[N]++)&/@S])&

[Try it online!][TIO-kx43ai2d]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kx43ai2d]: https://tio.run/##fVJhj5pAFPx@v2JPEqN1qbvq6Sm31zW0TZq01gaTxhBCFkGlVSDItV45@Ov2IXBg7nJ@cd57w@zM292LaOvsReSuxOkzYqeWunNEyKfKnC38T8cgdA4H1/e4FoWut9GCnRtxSdHYtMtjgmmitCRuMqJIPGCSrlPDAOiaH2YPe8sJf0yYC7XK4gT@Zoy2m12uKT@37s7RyR207thXx9tEWz6HydSzOdeaTdBUr@Gbp6e5rgMJgyy7ZuHqD5C@h8Bp41Y@Mozu@9g18dHEj@aEJJN77a8brbb6kkn8UXHxwYmwxI9siYVtZ6gDcP@wy@C7DPrnLrCP6TffTpf41@Zf1rknZyMz4Mu0jQ@ejVtUlsCB1OZqOg0Cx7MXfgpUbOIva70wjeMYWglIqAmoqulC/HY@hn6QUizpM0OWsx0B6HTO2zDaTdh8l1/FcQMOQbSBrxA6w14FgxzCCpCooFXBVQXtRgIY1JwIuahfCkIlSnVYAAoQHeUVJIYqqEaiPBp2BhIyrXhQ1WbieZYfRnujqgzQ8JbUz7u9ITdF7UOkMklhpjceDcaVdNbpD17jZ9rWs12YWIgS@FXbst5wP64qgfovdpn1rYtUa0QuIw7fuos8@EWyUixPZdV3Pqg8i/o11Ui0NFkLltuib6Sk9IVyNlnDZFhfgEzHxWspboG88iSyeMeClg9I3R88iHxWXFv9ynp1OdJIktN/ "Wolfram Language (Mathematica) – Try It Online"