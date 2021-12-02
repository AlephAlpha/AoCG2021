# [Pari/GP], 98 bytes

    s->vecmax([vecmin([#[1|k<-[j..p=#s+a=0],p*=a+=I^(Vecsmall(s)[k]%69)]+j-i|j<-[i..#s]])|i<-[1..#s]])

[Try it online!][TIO-kwod74cc]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwod74cc]: https://tio.run/##Xc09C4MwEAbgvxIihaSaUJdCoXGJCJ3cuoQUgmiJXxymlBb87/YUp07vPS/cHbjJiycsDVFLENm7rgb3YWZNPzITmXTursK0UoKKQuzUySZwVC5Wtwe711UYXN@zwE1nD@cLt3Er/NzihpcyCtby2SPSHYsD6L8sEJERmPz4wpGuoKTBIzwhhmqaEFrm@RalLoui@IPWei/Qm9ZaIym@@AE "Pari/GP – Try It Online"