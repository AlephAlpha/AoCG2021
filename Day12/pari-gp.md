# [Pari/GP], 32 bytes

    a->t=0;[t=[1-t,t*x][#d]|d<-a];t'

[Try it online!][TIO-kwhmjqm0]

I think this is the simplest challenge so far.

If the length of the direction string is 1, you go from an octagon to a square or vice versa. If the length is 2, you either go from an octagon to another octagon, or from a square to invalid.

Here we use the variable `t` to store the state of the current tile: `0` means octagon, `1` means square. When the direction has length 1, we just change `t` to `1-t`. If the length is 2, we multiply `t` by `x`, so `0` remains `0`, while `1` becomes a polynomial. If `t` is a polynomial, `1-t` and `t*x` are also polynomials. So invalid states are represented by polynomials.

Finally, we take the derivative of `t`. The derivative of a constant is `0`, which is falsy, while the derivative of non-constant polynomials are truthy.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwhmjqm0]: https://tio.run/##K0gsytRNL/ifpmD7P1HXrsTWwDq6xDbaULdEp0SrIjZaOSW2JsVGNzHWukT9f2JBQU6lRrGCrp1CQVFmXgmQqQTiKCmkaRRrauooREfHAgmlYCUIFQ6h/ZR0FJRcQYRfOJh0hYqDxYIhZDiSPFx9MIjAbQpcGRYD0QxBNh/ZQKBIbKzmfwA "Pari/GP – Try It Online"