# [Pari/GP], 35 bytes

    a->t=0;[t=[1-t,t*x][#d]|d<-a];!(t')

[Try it online!][TIO-kwg0xjzb]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwg0xjzb]: https://tio.run/##K0gsytRNL/ifpmD7P1HXrsTWwDq6xDbaULdEp0SrIjZaOSW2JsVGNzHWWlGjRF3zf2JBQU6lRrGCrp1CQVFmXgmQqQTiKCmkaRRrauooREfHAgmlYCUIFQ6h/ZR0FJRcQYRfOJh0hYqDxYIhZDiSPFx9MIjAbQpcGRYD0QxBNh/ZQKBIbKzmfwA "Pari/GP – Try It Online"