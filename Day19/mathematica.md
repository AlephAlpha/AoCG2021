# [Wolfram Language (Mathematica)], 167 bytes

    Min[Max[Last/@Tally[Join@@MapThread[Range,{#-r,#-1}]]]&/@Pick[r=Range[n=Max@#];{a,b}=#;s=Select[Range@Tr@r~Tuples~n,#r&&#[[b]]-b#[[a]]&],Max/@s,Min[Max/@s]]]&

[Try it online!][TIO-kwrlqdps]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwrlqdps]: https://tio.run/##LY5BasMwEEWvIhB4NcbYWQYVrUsNIfFumMXYVRpRRw2yAilC2XaZXKbnyhFcue3qv@Ezb@bI4WCOHOzA816oubUOW77gC0@h0h2P4yc@f1indcun7uANv@KW3ZuBKEsPsqwTERWV3tjhHb367dCp7NCS1pGhT0o@bl/rSe3MaIbwt647r/21O59GM10dyMf92xeFROyJyj5PGTmLCbKp0hP8P5ZxuTdvvHUBpSifxB4lkShEpUWMsYE6gYgraNKSsQbRLJBzlVKafwA "Wolfram Language (Mathematica) – Try It Online"