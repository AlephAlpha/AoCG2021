# [Pari/GP], 181 bytes

    a->m=vecmax;l=n=m([m(b)|b<-a]);forvec(v=[[i,k=n^2]|i<-r=[1..n]],u=v-r;if(![v[b[1]]>u[b[2]]|b<-a],d=Vec(sum(i=1,n,(x^v[i]-x^u[i])/(x-1)));if(#d<k,l=m(d);k=#d,#d-k||l=min(l,m(d)))));l

[Try it online!][TIO-kxa6v8fs]

Brute force. Extremely slow.

Let \$n\$ be the number of jobs. Loops over all tuples \$[v_1,\dots,v_n]\$, where \$i\le v_i\le n^2\$ (a better but longer upper bound would be \$n(n+1)/2\$). \$v_i\$ represents the ending time of job \$i\$, so the corresponding starting time is \$v_i-i\$. For each tuple, checks if it satisfies the graph.

Now we can write job \$i\$ as a polynomial \$x^{v_i-i}+\cdots+x^{v_i}\$. Let \$d\$ be the sum of these polynomials, with \$i\$ running from \$1\$ to \$n\$. Then the ending time of all the jobs is the degree of polynomial \$d\$, while the number of workers is the largest coefficient of \$d\$.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxa6v8fs]: https://tio.run/##JY5Ra4QwEIT/Snq@JLC5I95jXH9GX5YVYlNLUFOxVTzwv9sN3Zf5ZhaGWcKa7NdyDQqvYNsZ98@PORx@woyzpln35uwbG9j44XuVp96RKMGIuav5TI1dkdz9nplhw92uPg36jXbqyTG3m2jN/F8BEd@l4GebdUIHGfTR7ZTYHt0mYh76sM4YUyqq2IwwyYRo/IhVhCra8TwlSVlPUPJyfrrCskwvHZRt1bKm/Ct4K@amBh2MAUVENSjHQk9QsqZErpCA6JOZzfUH "Pari/GP – Try It Online"