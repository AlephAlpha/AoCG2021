# [Wolfram Language (Mathematica)], 118 bytes

    -Max[Count@4/@Select[Tuples[Range@4,l=Length[s=ToCharacterCode@#~Mod~11]],FreeQ[Tr/@Rest[I^Subsequences[s+#]],0]&]]+l&

[Try it online!][TIO-kwmz4rzz]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwmz4rzz]: https://tio.run/##LYxdC4IwGIX/ylDwRsUEL3UMhCBIKPVuTFj6@gE6a5sSRP71ZdHF4fBwHs7EdQ8T10PNTYsS42f8SdN5EZpEASlghFrTcrmPoGjORQck8sbkDKLTPVVJOac9l7zWINO5AWJv2dxsYciYd5QAV1rKgOSgND1VxXJT8FhA1PuXcu3dOTCHMXd0zEUOQlMb@Ri1dF@QgwKCXlZVYbyucWx5yMIx/tcPq3jF31hv8wE "Wolfram Language (Mathematica) – Try It Online"