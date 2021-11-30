# [Pari/GP], 502 bytes

    p->a=[[j==16&&k|j<-[1..26]]|k<-[0,w=1]];c=[[],[]];n=[1,1];while(sum(k=1,2,#c[k]||Vec(p[n[k]])[1]!="r")&&w,for(k=1,2,while(w=n[k]>0&&n[k]<=#p,(g(u,v)=if(0<t=s[u]-96,a[k][t],eval(concat(Vec(q)[u..v]))));s=Vecsmall(q=p[n[k]]);i=s[2]-96;v=if(i-14&&i-7,x=s[5]-96;7,5);if(i==7,while(s[v]-32,v++);z=g(5,v-1);v++);i-3&&y=g(v,#q);i-5||a[k][x]=y;i-4||a[k][x]+=y;i-21||a[k][x]*=y;i-15||a[k][x]%=y;i-7||(z>0&&n[k]+=y-1);i-14||c[3-k]=concat(c[3-k],y);i-3||if(m=#c[k],a[k][x]=c[k][1];c[k]=c[k][2..m],break);n[k]++)))

[Try it online!][TIO-kwlndea3]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwlndea3]: https://tio.run/##dVPRkqIwEPyVHNZRcCYUAYG1MPsZ95LKQ0DxEFQUxXWLf/cmhKB7dctLujuTnp6popHnkmybR4HYoyHvknG@Y4zGtl31uxXh1POCWIi@AuzjG6NCpDkUCcwBHRinmIr09qesN0573TsVozjAs5xXou9/b3Kn4QfAwuVU/GDW2XJt@4aL43ms1C9vTBW9@7atzhWbNdjZOlfcuawsHH91YS2/CrKMsYR7fhF408nayY@HXF4c1ebk8qvndcKFL20ZSO1e1rVzYiZAWoJJoEzSTrmWhC5suyQJ/oCLaLhIcAR1cMdYMkZreSdIGOBuPnfTT7Z1ItwR6qYDL0lo23cQOzw7KRr1/ZDwQ7A70MVE5wMP6CT8GgT6fPBzEJK@dz7NIuCRaqWS9n3OQ1IJNs6sGb4PGfoeMu/ZsHVs@isCS0/VqUngeXuBs/NGVm46@M9hWw/ZNPXdKTDi3GoPa0QtjAYQGNAocM47JA3IDMgNWFsCHKx2c0H1aAGwROGEpZb31xo1iCYK77afgBsjS91SrtfwkFBTAXjS5ahrcxokhjQofvOf/m@RHw3sCPF17rFxsEwWS2OneLj4t1L5ZWMsUDNEffjMNrJvMi4Nlij8sielZS@5C@S/jhD/f7t6qJfk2kCnzp7bW5hc8rno6brWUabYuj39ZgJKv3gptQA1fg5G6NKCf@nxFw "Pari/GP – Try It Online"