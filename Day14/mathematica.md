# [Wolfram Language (Mathematica)], 387 bytes

    (Clear@A;P=ToExpression@StringSplit@#;S=A/@{Z=0,1};(#@_=0;#@p=#[[1]];#@i_?NumberQ:=i;#@C={};#@N=1)&/@S;While[#@C!={}||P[[#@N,1]]=!=rcv&/@Or@@S&&Z<1,While[0<#@N<=Length@P||0>++Z,P[[#@N]]/.{i_,x_,y_:0}:>Switch[i,set,#@x=#@y,add,#@x+=#@y,mul,#@x*=#@y,mod,#@x=#@x~Mod~#@y,jgz,#@x>0&&(#@N+=#@y-1),snd,(1-#&/@#)@C~AppendTo~#@x,rcv,If[#@C!={},{{#@x},#@C}=#@C~TakeDrop~1,Break[]]];#[N]++]&/@S])&

[Try it online!][TIO-kwj059ls]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwj059ls]: https://tio.run/##fVFrb9owFP3eX@ESKYJhRgwUysPMlG3SpI0xBWkSUYQcYsArkCikG10If53dNKQO6kS@5Jz7OPee6w0PV2LDQznnp8@InorDteABG3THdOJ92vuB2O2kt2VmGMjt0vTXMmRa16SDKoum1MAk7hY1NqNGV2M@1SyL2DZAOfsweto4IvjRoRL4kEYx/EaUlPQqM7s/V3ItLIjfQuJwGFuARxh66S0N5r@h5nvAmKnr0x7BabHRg5Ie/Sq2y3DFxoeD0S@Xpzhtte3q@0jO8H6Gn2cdI@70zT8ynK8siXcixBrbU409Y@66CS6/kM3TOiHvUuK556r98ZvnHpPYr@XfJNY3dB08jl66KqSEd1sXF0lFgy21EhseB74vtu7Eg6Y9hu3xl0VmDUcRBGOQGcbQPjxO@KP4GHj@keCHQPBHy07uZY3sctlOLmOXdHiHKruJogLMQaSAbxB6gTUF/RTCLMQVdBScK@gWYsCgJkIkUT0TBMYzdbgE8hFppQxsA/NVimej4XwgUSGqDlgux19z6TBSaynqo@a9kZ93f2fcnbkHljIn52Vq7VajraSTSL3xv/pE23ldFzIOIgZ86lrOle3binFUf3PLJO5cuFog49Ji89pbpMYvnGViqSsnf/OG2pnnnylXRLIlc8bStcgVl4S8UU4yC8g08weokHYhjk//AA "Wolfram Language (Mathematica) – Try It Online"