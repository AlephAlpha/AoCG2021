# [Pari/GP], 78 bytes

    s->a=b=0;#[1|d<-Vec(s),if(a,a=0,d=="!",!a=1,b,d==">"&&b=0,d=="<",!b=1,d=="{")]

[Try it online!][TIO-kxe2a983]

When your language doesn't have regexp or any string pattern matching built-in...

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxe2a983]: https://tio.run/##ZY1NCsMgEEavolMICYyQrKseo5uQheanBEoqSTfBevZ0TG0bKOjwzXuj48w8iqvbBqa2RWijrCrPp7p6dlJc@jZfChyH3KBRJXZKAQfkRlVo905DltlkJBlLJmYPRbMZ525rvjChmZvH6UERYgNsoG8LZDX4AMjAex9CSgF9@EKMJ7o3kT@iEzEaDzc9jAn/6kfyHRzrUXIdgW1JUMM1tbSX5iJY@0VKOd1pHiVta4rtBQ "Pari/GP – Try It Online"