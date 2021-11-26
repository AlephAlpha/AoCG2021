# [Wolfram Language (Mathematica)], 80 bytes

    Map[t=0;((t=⌊(3Mod[t-#,8]+9)/5⌋+#)&/@Mod[2ToCharacterCode@#+2,30];t~Mod~8)&]

[Try it online!][TIO-kwed5bfl]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwed5bfl]: https://tio.run/##JYlLCoMwFACvEhIQxYiiFCxiEXzLCCU0K8ki@EEX1iLZiR6g9ZReJNV2VsPMoHTXDEr3lTItSk2hXqVOg8S2dbpvbzsqxrrUHqGxdK@Of9m3j0scy8/OHj7GvFOTqnQz5WPdZMQNaRTIRK/HXmPHkuY@9U9dEuTdUFsSKZGF/AzNMxaMYYow5wBwChMcfkUcAF4omo/J@ZmAMSH@ygA4FwIvi/kC "Wolfram Language (Mathematica) – Try It Online"