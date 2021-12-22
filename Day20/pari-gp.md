# [Pari/GP], 81 bytes

    f(a)=#a&&if(a[1],sum(i=2,#a,f(a[2..i])*f(concat(a[1]-1,a[i+1..#a]))),a[#a]+2==#a)

[Try it online!][TIO-kxgwjobf]

A port of [@G B's answer](https://codegolf.stackexchange.com/a/239887/9288).

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxgwjobf]: https://tio.run/##XU3RCoMwDPyVoiB21mLqkw/uR0ofguAobK647WFf3yWtMjdomrvkchdw9e0lxDjXKMcSq8oTsuDU43Wr/WhUiYonRmvv5Gmup/sy4TNpWlBofQNal@iklMQINGYkIxkxhOu7RtGeRVj9QieiYFIIzpJKWNsp0TkCQD0/ZtSH4Vs9z0xaAxeJgWhPLQ1ZQ8ikH3acrpLbZglbEGz8EJh9sqfhQZ/TdtERHFTmd/OPnZPxAw "Pari/GP – Try It Online"