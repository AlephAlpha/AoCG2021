# [Wolfram Language (Mathematica)], 111 bytes

    Min[p=Position;Count[Or@@@#,1<0]&/@Outer[#!=##2&&{1,1,-1}.Norm/@{#-#3,#3-#2,#-#2}==0&,#~p~1,#~p~2,p[#,1|2],1]]&

[Try it online!][TIO-kx5r6nzh]

[Wolfram Language (Mathematica)]: https://www.wolfram.com/wolframscript/
[TIO-kx5r6nzh]: https://tio.run/##lU67agMxEOz9FQoLqvZy2nWZyAhcJ3YvVBzBJiruwUWuZPnXL8rJOXNNIDAss8Ps7LRN@Dy1TfAfzXQWenrznR30sf/ywffdy76/dMEeRmMMIL0qJ2tzuITTaOFJA7CUkZCwovT83o9tbSJUsEXYVsCYKSetlUS4DTeaJ@Ngc9KVHZJzcjqOPj8AUe3E2YJzQorabESMkVLCjciMUGTw78qZF8yC@I@wZKqyolB3yw@dQY8but8sjmLidTG1cnEJWUXRXxo/OiylStM0fQM "Wolfram Language (Mathematica) – Try It Online"