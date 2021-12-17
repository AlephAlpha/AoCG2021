# [Pari/GP], 181 bytes

    a->m=vecmax;l=n=m([m(b)|b<-a]);forvec(v=[[i,k=n^2]|i<-r=[1..n]],u=v-r;if(![v[b[1]]>u[b[2]]|b<-a],d=Vec(sum(i=1,n,(x^v[i]-x^u[i])/(x-1)));if(#d<k,l=m(d);k=#d,#d-k||l=min(l,m(d)))));l

[Try it online!][TIO-kxa6v8fs]

Brute force. Extremely slow.

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kxa6v8fs]: https://tio.run/##JY5Ra4QwEIT/Snq@JLC5I95jXH9GX5YVYlNLUFOxVTzwv9sN3Zf5ZhaGWcKa7NdyDQqvYNsZ98@PORx@woyzpln35uwbG9j44XuVp96RKMGIuav5TI1dkdz9nplhw92uPg36jXbqyTG3m2jN/F8BEd@l4GebdUIHGfTR7ZTYHt0mYh76sM4YUyqq2IwwyYRo/IhVhCra8TwlSVlPUPJyfrrCskwvHZRt1bKm/Ct4K@amBh2MAUVENSjHQk9QsqZErpCA6JOZzfUH "Pari/GP – Try It Online"