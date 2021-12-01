# [Wolfram Language (Mathematica)], 378 bytes

    (Clear@A;P=ToExpression@StringSplit@#;S=A/@{0,1};Z=1>0;(#@_=0;#@p=#[[1]];#@i_?NumberQ:=i;#@C={};#@N=1)&/@S;While[#@C!={}||P[[#@N,1]]=!=rcv&/@Or@@S&&Z,While[Z=0<#@N<=Length@P,P[[#@N]]/.{i_,x_,y_:0}:>Switch[Y=#@y;i,set,#@x=Y,add,#@x+=Y,mul,#@x*=Y,mod,#@x=#@x~Mod~Y,jgz,#@x>0&&(#@N+=Y-1),snd,(1-#&/@#)@C~AppendTo~#@x,_,If[#@C!={},{{#@x},#@C}=#@C~TakeDrop~1,Break[]]];#[N]++]&/@S])&

[Try it online!][TIO-kwj9m6vt]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwj9m6vt]: https://tio.run/##fVFhb9owFPzeX@ESKSrDjBgoFFIzU7ZJkzbGFKQJoihyiAGvQKKQbnRp8tfZS9M0QZ3Il9x773x@d97ycC22PJQLfvyM6PFqtBE8YEN9Qqfep4MfiP1eejtmhIHcrQx/I0Om6AYdNlikYRLrc0oGmn6lMJtqusJ8qpgmsSyA0v4wftg6IvjRpxLqEY1i@I0pqaoNZug/13IjTOhfwuDpaWICHmM4Sy9psPgNnO8BY4aqznFGnVPtFii39KvYrcI1m@DsjGU13kfSxgcbP9p9Le4PjD8yXKzNGVXYoy7xXoRYYQc6w9x1U1QDuH3YpPBdCr3nLrAPyTfPTWb41@pv2hloqgrWxsCvkyre71x8ReoKrKZU2SgZ@r7YuVMvASq28Zdl7gZHEbRikBjFoDpKpvxefAw8PyH4LhD83rTSiMyxVatZaRhWVYX4G@wiiipwCyIVfIHQM2wW0M8ghIN4AZ0CLgroVmLAoCZCJFErF4SK5@qQAPIR6WYVWIbKL0Y8vxpCA4k6KXhQlWb8dZZdRprdovRR50Yr33dzrV2/1B5Yyp28LNPsddu9QjrttNr/46fazuu6MHEQ0eAr0nLObN8rKo5ab7JM@86JqyXSTi12zr1FZvzEWS6WuXLKmbeLnXn5mUokki9ZMpatRc64JOSNcjpZwqRTDqBOepU4Pv4D "Wolfram Language (Mathematica) – Try It Online"