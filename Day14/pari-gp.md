# [Pari/GP], 443 bytes

    p->a=[[j==16&&k|j<-[1..26]]|k<-[0,z=1]];c=[[],[]];n=[1,1];while(sum(k=1,2,#c[k]||Vec(p[n[k]])[1]!="r")&&z,for(k=1,2,while(z=n[k]>0&&n[k]<=#p,s=Vecsmall(q=p[n[k]]);i=s[2]-96;v=if(i-14,x=s[5]-96;7,5);i-3&&y=if(0<y=s[v]-96,a[k][y],eval(concat(Vec(q)[v..#q])));i-5||a[k][x]=y;i-4||a[k][x]+=y;i-21||a[k][x]*=y;i-15||a[k][x]%=y;i-7||(a[k][x]>0&&n[k]+=y-1);v-5||c[3-k]=concat(c[3-k],y);i-3||if(m=#c[k],a[k][x]=c[k][1];c[k]=c[k][2..m],break);n[k]++)))

[Try it online!][TIO-kwj9evdw]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwj9evdw]: https://tio.run/##dVPRbqMwEPwVH9EhuBqESUKKiPsZ92L5wRDoEUjiQMuViH/PrTGGtLry4pnx7nh2JaRoSu9V3gtE79J7EZSxI6Uksu1qOO49Rnw/jDgfKsABvlHCeZJBEccM0JkygglP/v4p69xp309ORQkO8SpjFR@G33nmSHYGzF1G@A9qNZZr2zdcXJqpUnfeqCp6CWxbnXu6kril0N2eRF07V2pMkpK2LOReHCUdLQun9MgGf4C2HbUd3kKJt7btXt0G@x6uOnWFBfSznuO8E7WTXc6ZeHNUvKvLOt9fXbnrqtbtMIyVH5z2QDczfRp5SGbh1yiQpeHnKOyGwZkEMw60esRNOmWesbVXcToF0Az3Y@hhgMgnOq4OmxCKwOYSdWoS@v6J47TJReUmo/0TRL8LKeveKTBizGrPB0QsjEYQGiAVaLIOCQNSAzIDDhYHB6vN31A9WQAs0XrGQsun9xpJRHYKH19vgKWRhX5SHA7Q6BFTAXjWxaRrcxLuDJEoeg4W/@dtsB3ZBeLr3NPDYbzbxMZO8fXma6XyS6dYoKaIBPCZbaTfZIwNFmj9aU9KSx9yFyh4HCH6/3b1UA/JtYFOnS7b25hcYln0fF3rKHNs/Tz5ZgJCPnkptQA1WgbzSGzBz3T/Bw "Pari/GP – Try It Online"