# [Pari/GP], 45 bytes

    a->i=1;iferr(chinese([Mod(i--,b)|b<-a])',e,1)

[Try it online!][TIO-kxjz7jc2]

Taking holes as 1.

Tries applying the [Chinese remainder theorem] built-in. If it throws an error, the bus company is cheating.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxjz7jc2]: https://tio.run/##NUxLDsIgEL3KpBshGRa0NA3R9gaeoGFBFZTEtATdmHh3HKgm83ufedGmIG4xexizFVMY5TF4lxK73MPqno7N5@3KghC48M9yEtbwAzqUPNsYH29mQUwQU1hfdDYFNOCZ5RxhngcE2VHX6nVdXUHakExHSxhBkViJMrT@i6T0CJRRHuUvqhqJG8res9UeX31toXdCGcPzFw "Pari/GP – Try It Online"
[Chinese remainder theorem]: https://en.wikipedia.org/wiki/Chinese_remainder_theorem