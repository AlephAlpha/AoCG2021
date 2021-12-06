# [Wolfram Language (Mathematica)], 61 bytes

    Sum[#[[i,Mod[(i-1)#3/#2,Tr[1^#[[1]]]]+1]],{i,1,Length@#,#2}]&

[Try it online!][TIO-kwumoxim]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kwumoxim]: https://tio.run/##jZFNCsIwEIX3PUVgQBQjdiIiRZQeQEHQXaiQaqtZVEHqKuTsNVYrY1t/QgjfJC9vJplM5cckU7neqSJls2J9zSRIqfnyvJddPcAejIYg@OYicesOMHKj71ZuNEe@SE6H/BgCB2GjTqHYzDPG5wzdtNxjxoFP@B5aO/W8uFI@xSXUJ3F4KetcavyGA1KoNK/9pg@2@eAfPthWcy1RvbYPNTc1rVnw6//8zNX29ntHVhd9yqUBsGwwZ6kEiCLWYWEYukYp0lLHQUAC8c6jit0FQZjuB0EZxMQ1JqIHjwlPKi6T2eIG "Wolfram Language (Mathematica) – Try It Online"