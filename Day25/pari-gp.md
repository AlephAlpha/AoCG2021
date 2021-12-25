# [Pari/GP], 114 bytes

    a->l=[[m[1,],m[#m,],m[,1]~,m[,#m]~]|m<-a];[i|i<-[1..#a],vecsum([#[1|f<-concat(l),e==f||e==Vecrev(f)]|e<-l[i]])==8]

[Try it online!][TIO-kxl8wj7p]

A port of [@Neil's answer](https://codegolf.stackexchange.com/a/240143/9288).

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxl8wj7p]: https://tio.run/##hVPBioQwDP0VwYtCOzS3hdr9jL2EHER0EeysuLNzKvPr7riMmrTKQmn1kZeXviZjPfX6c5y7zM21fh8cokdQpDzm/u9QQI/lyD09KPhK12SxD32lES6XvCZ1b5vvH19gjhC6Sjdf16a@FUOpWue6EJ77R9tM7b3oSgptpQfsiUrn3mgep/56K7oC0agM1rV82/33BdoFN2vAFrOBWwwwBKwIWBapDDeeWXk8k0kycQQYwvMYprZzFzXDSedqokorKRLhMVzfvNSECWmUFWkit89YESKdhJMqD3mRfvq2IN02wsm07rMXMKwD0p6Ao7vt@65mpCfR3f7NnfbNAWvvkogXeQJJTDQlkX7a23DQJVwtvS1Ib6OZOJxS0V7PWS/nXw "Pari/GP – Try It Online"