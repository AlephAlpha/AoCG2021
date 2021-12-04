# [Pari/GP], 100 bytes

    f(a)=#a&&0<(l=#a-a[#a]-1)&&g(a[2..l],a[1])
    g(a,b)=if(b,sum(i=1,#a,f(a[1..i])*g(a[i+1..#a],b-1)),!#a)

[Try it online!][TIO-kwrx7cvh]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwrx7cvh]: https://tio.run/##XY7PCsIwDMbvPkV1MBrNxtKdBOeLlB6yg1KYUqYefPqadhtToW2@L39@aeDRV9cQ40UzdAWXZXPSg4iKbcGuIijLq2Zr6npwyJYcbMRjD52/6B4fr5v2HWHBKARLde0d7NOEP4gRBPYCAdwWDJFDGN6aVXVWYfT3p8hdMjuV1gMqaxtUjRNBEqeTnMTjcb1typlcpnSlmcS2EnIy9Ygy@aVF56lMm5E0L6J14UQxKdFO/OUf3@Kry/xW/rVzED8 "Pari/GP – Try It Online"