# [Pari/GP], 467 bytes

    p->a=matrix(2,26,i,j,j==16&&i-1);c=[[],[]];n=[1,1];while(![m<=0||m>#p|m<-n]&&sum(k=1,2,#c[k]||Vec(p[n[k]])[1]!="r"),for(k=1,2,(g(u,v)=if(0<t=s[u]-96,a[k,t],eval(Strchr(s[u..v]))));s=Vecsmall(p[n[k]]);i=s[2]-96;v=if(i-14&&i-7,x=s[5]-96;7,5);i-7||while(s[v]-32,v++)||z=g(5,v++-2);if(i-3,y=g(v,#s);i-5||a[k,x]=y;i-4||a[k,x]+=y;i-21||a[k,x]*=y;i-15||a[k,x]%=y;i-7||(z>0&&n[k]+=y-1);i-14||c[3-k]=concat(c[3-k],y),if(m=#c[k],a[k,x]=c[k][1];c[k]=c[k][2..m],n[k]--));n[k]++))

[Try it online!][TIO-kx44wzmm]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kx44wzmm]: https://tio.run/##dVNdj6IwFP0rHcyasraGouAYrH9ik31p@lDxY1BQAsqq6X93bylFZzLDi@fc3nt67mksVZXRXfnYIv4o6VLxQp2r7IpDEsYkI3uy55zFw2FGmZ@kXAhJhJTJkQtGmEz@fWT5Br@JYsEDrYvloNTFgh7lcFhfCnzgjIRkkIqD1PrvJsWlOAKWvmDyjXuV55Ptqera8A5fSOPzbIuDxZnX4iLpPCZKHMhZkk2jcvznXKUfFYaj8biRPnxJzUG3LlSe9@JJBsOhGU4aowbWp2aBGbnCQdQezEgEfXSmtd2gFo2kk5A0o5Gv9Z3vcGQwDaHLKEzIDWoNGdRmLNLa2LpKfgM2dWzU0pA5/rvlrO/@1XK4E9@XwXBo3MKICdZY1DoVE3qQPD0dU3XGlpGbT8BBwdsUSXetwZBhYn4tCcfjQhIjSSnE0mqPfP@hyjK/4S1BQnj1cY2YR1ALQgdKA6q0QcqBlQOpA2tPgoJXb84o7yQAZmjSY2XLxSVHJWIzg/e7O@DSlZW9Uq3XMEiZ6wDc11VXt@IsnDlSovg9eOq/R0HUshPYt767i8P5bDp3coZPpl87jd6qswXVFWIBfC6N1Q8e5w4rNPmUk6mtXnxvUfC6Qvx9unapF@dWwLpePdObOl/qGXR/nFsrvW17PfthA8Y@aZnqFqrxczHK5vaduzCDL69o3F9th632Dcw8YnvQ5f7MPHyKBB78Ox//AQ "Pari/GP – Try It Online"