# [Pari/GP], 495 bytes

    p->a=[[j==16&&k|j<-[1..26]]|k<-[0,w=1]];c=[[],[]];n=[1,1];while(sum(k=1,2,#c[k]||Vec(p[n[k]])[1]!="r")&&w,for(k=1,2,while(w=n[k]>0&&n[k]<=#p,(g(u,v)=if(0<t=s[u]-96,a[k][t],eval(concat(Vec(q)[u..v]))));s=Vecsmall(q=p[n[k]]);i=s[2]-96;v=if(i-14&&i-7,x=s[5]-96;7,5);i-7||while(s[v]-32,v++)||z=g(5,v++-2);if(i-3,y=g(v,#q);i-5||a[k][x]=y;i-4||a[k][x]+=y;i-21||a[k][x]*=y;i-15||a[k][x]%=y;i-7||(z>0&&n[k]+=y-1);i-14||c[3-k]=concat(c[3-k],y),if(m=#c[k],a[k][x]=c[k][1];c[k]=c[k][2..m],break));n[k]++)))

[Try it online!][TIO-kwros5gp]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwros5gp]: https://tio.run/##dVPRkqIwEPyVHNZR4UwoAgJrYfYz7iWVh4DiIagoiusW/@5NgKB7dctLejqTnp6uolbngm7rR474o6bvigux45xFtl12uxUVzHX9SMquBOyRG2dSJhk0SSIAHbhghMnk9qeoNri57nHJGfHJLBOl7LrfmwzX4gBYOoLJH9w6W45t30h@PI@dw8sb103vnm3rc8VnNcFbfCWtw4sce6sLb8RV0mVEFNyLiySbVlU4Ox4ydcF6zMkRV9dtpQNf0nCgmr2qKnzixkBSgIivRZJWqxaULWy7oDH5gIuwv4hJCH007rpxI9FKGviknc@drvvkWxxqTH3o0goBuQPXktlJPwu7rrf3IfkdysVUzvvaZxPxqyfY88HPnoC5@NOkAI8o07IMhDIR0FLyceGhIneHgIs979MmZrQuIOxEn0Phu@5ekvS8USWE02vPIaaHquvqjnOChLCawxoxi6Ae@AbUGpyzFikDUgMyA9aWBAWr2VxQNUoALFAwYTXQ@2uFasRijXfbT8C1odUwUq3X8JAy0wF44tXID@LMj01Ro@jNe@q/hV7YV0ewP/geB/vLeLE0croOFv92ar10tAVsipgHn0kj/cbj0mCFgi85aS598Z0j73WF6P/pDku9OB8EBtfpM72F8aWeQU/X1WBlsj2MZ99swNgXLc3mwEbPxShbWvATPf4C "Pari/GP – Try It Online"