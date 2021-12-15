# [Pari/GP], 462 bytes

    p->a=matrix(2,26);a[2,16]=1;c=[[],[]];n=[1,1];while(![m<=0||m>#p|m<-n]&&sum(k=1,2,#c[k]||Vec(p[n[k]])[1]!="r"),for(k=1,2,(g(u,v)=if(0<t=s[u]-96,a[k,t],eval(Strchr(s[u..v]))));s=Vecsmall(p[n[k]]);i=s[2]-96;v=if(i-14&&i-7,x=s[5]-96;7,5);i-7||while(s[v]-32,v++)||z=g(5,v++-2);if(i-3,y=g(v,#s);i-5||a[k,x]=y;i-4||a[k,x]+=y;i-21||a[k,x]*=y;i-15||a[k,x]%=y;i-7||(z>0&&n[k]+=y-1);i-14||c[3-k]=concat(c[3-k],y),if(m=#c[k],a[k,x]=c[k][1];c[k]=c[k][2..m],n[k]--));n[k]++))

[Try it online!][TIO-kx7ghvwz]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx7ghvwz]: https://tio.run/##dVPRjqIwFP2VDmZNWVtDq@gYrD@xyb40fagoDisoAWXV8O/uLaXgTHZ48Zx7b0/PPY2FLlN6KJ4JEs@CbrTI9aVMb5gTvvAjLTlhCyVYFAspFZFKRSchGWEq@vuRZnv8JvO1CJom34yKJl/TkxqPq2uOj4IRTkaxPKqm@b2PcSFPgJUvmXoTXun5JDmX3Rg@4CupfZEmOFhfRCWviq4WRMsjuSiyr3WGf13K@KPE0JpOa@XDF1UCdKtcZ1kvHqVwmJvDUW3UUsrm43FKl@QGjbBtLEkIc3TZNHaDStaKzjipJxO/aR7igEODKYcpozAjd6jVZFSZY2HTGFs3Je7A5o5NWsqZ4z9bzvrpHy2HO/FjE4zHxi0cocxIMlCJ5YwelYjPp1hfsGXk7hNwkIs2RdJdazBkGJlfS/h0mitiJCmFWFrtie8/dVFkd5wQJKVXnXaIeQS1gDtQGFDGNdIObB2IHdh5ChS8an9BWScBMEWzHmtbzq8ZKhBbGvzn8ABcuLK2V@rdDg5S5iYA93Xd1a0440tHCrR4Dwb99zAIW3YG@9Z3dzFfLecrJ2f4bP510uhtO1tQ3SIWwOfS2H7jceWwRrNPOZna9sV3goLXFRb/T9cu9eLcCljX2yG9ufOlh6D7dmat9Lbt9eybDRj7pGWqCVQXw2KUrew7d2EGX17RuL/ZCVvtB5h5xLbR5T5kzgeRwIN/5/Mf "Pari/GP – Try It Online"