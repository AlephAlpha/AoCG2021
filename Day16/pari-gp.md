# [Pari/GP], 459 bytes

    p->a=matrix(2,26);a[2,16]=1;c=[l=List(),l];n=[1,1];while(![m<=0||m>#p|m<-n]&&sum(k=1,2,#c[k]||Vec(p[n[k]])[1]!="r"),for(k=1,2,(g(u,v)=if(0<t=s[u]-96,a[k,t],eval(Strchr(s[u..v]))));s=Vecsmall(p[n[k]]);i=s[2]-96;v=if(i-14&&i-7,x=s[5]-96;7,5);i-7||while(s[v]-32,v++)||z=g(5,v++-2);if(i-3,y=g(v,#s);i-5||a[k,x]=y;i-4||a[k,x]+=y;i-21||a[k,x]*=y;i-15||a[k,x]%=y;i-7||(z>0&&n[k]+=y-1);i-14||listput(c[3-k],y),if(#c[k],a[k,x]=c[k][1];listpop(c[k],1),n[k]--));n[k]++))

[Try it online!][TIO-kx8a5h01]

Takes a list of lines as input.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx8a5h01]: https://tio.run/##dVPLjqMwEPwVD9FGZmOPMHkwEXG@YG8r7cXywSGPYQOJBYRNIv4928YYMqMZTtWv6uqy0KpI6UE/9og/NF0rnquqSK84JOHCj5UICVtIzuKEi4z/SssK@yST8YkLRpiM/72n2Q6/iHzFg6bJ1yPd5Ct6kuNxecnxkTMSklEijrJp/uwSrMUJsPQFky/cKzyf7M9F14YP@EJqn6d7HKwqXoqLpMsFUeJIKkl2tcrw76pI3gsMpdfXWvrwxSUH3jJXWdaTxykMh2Y4rg1bStlsPE5pRK5QmLeFiMyhj0ZNYy8oRS3pNCT1ZOI3zZ0f8NxgGkKXYZiSG@RqMirN2LxpjKyr5DeIZi6atGHIXPyzjVnf/aONYSe@r4Px2KiFEcoMJQOWDOzVlwonYkqPktx8Artb90i3zmDwLm47zxq3NeYTQ0Up2NFyTnz/obTObnhPkBBeedoi5hHUgtABbUCR1Eg5sHEgcWDrSWDwyl2Fso4CYIqmPVY2nV8ypBGLDP57uAPWLq3sSrXdwiBlrgNwn1dd3pKzMHKBRou3YOB/mwfzNjqDfKu7Wxwuo9nS0Zl4Ovvcafg2nSzIbhAL4HNubL7RuHRYoekHn0xu86R7j4LnExZfu2uPelJuCazqzeDezOlSg9F9ObNSetl2PfvmAsY@cJnsHrKL4TDKlvadOzODT69o1F9th832Dcw8YlvofB88DweSwIO/8vEf "Pari/GP – Try It Online"