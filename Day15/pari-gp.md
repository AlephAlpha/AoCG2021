# [Pari/GP], 114 bytes

    n->p=Pol(c=0);a=Map();for(i=1,n,if(q=mapisdefined(a,p),mapdelete(a,p),mapput(a,p,1));p+=x^(c+=(-1)^q)%(x^2-x+1));c

[Try it online!][TIO-kwm2v98h]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-kwm2v98h]: https://tio.run/##PYxLCgMhEESv4ibQjQrjbKVzg0BOIIifIEycnokBb2/GTRYF9epBsT@LfvHIgkbVd6bnvkGgBa2nh2dAm/cTChlVVclw0Ntz@cSUS00RvGJU1xLTllr6I3/b7MogWpbUHQRJoA26A2/Q3aq7nC6MeV4FiUWJ9QqfpTbIUBFx/AA "Pari/GP – Try It Online"