# [Pari/GP], 192 bytes

    m->while(a=0*m;a[,1]=m[,1];while(a!=b=matrix(#a,#a~,i,j,m[i,j]&&(a[i,j]+(i>1&&a[i-1,j])+(j>1&&a[i,j-1])+(i<#a&&a[i+1,j])+(j<#a~&&a[i,j+1]))),a=b);m!=n=a+concat([(m-a)[,2..#a~],0*m[,1]]),m=n);m

[Try it online!][TIO-kwhvs71c]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwhvs71c]: https://tio.run/##VY/BboMwDIZfhYKEnOFUyY5Nw32nPUDEwa3WLahhEaLadumrM0MJbIpi@fv/X5YdqffyPY6XzI5B1l8f/voGZNVTMORQNzZM1Sz6zp5soKH331AQFnRHjy0Gx7UpS6C5qcDXuiwZpGYUFbQLYyv1xP5Y0CxUKcDCfYlUHBECyZ6ECTvbWarOn92ZBnAQJAmHz/s9xxvkJaflGoHBdhweKcbrD1Am6yz2vhsgf@kOuTAPikCphfz1Nvx1LuwJzJzTqFGtXxn1jzXz4y2K2dzkbxPU7Os1n/xtQvLXCXzM@As "Pari/GP – Try It Online"