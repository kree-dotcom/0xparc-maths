describe all $n$ such that $(n-2)(n-3) \equiv 0 \pmod{72}$

Find the zero points but then because 72 is not prime we must factorize it and consider the situations in which the product of the two brackets could be equal to 72 also. 

The first solutions are $n \equiv 2 \pmod{72}$ and $n \equiv 3 \pmod{72}$

The factor pairs of 72 are 
1 and 72
2 and 36
3 and 24
4 and 18 
6 and 12
8 and 9

Now we must look for choices of $n$ which satisfy  $(n-2)(n-3) \equiv 0 \pmod{72}$ where $(n-2) \not\equiv 0 \pmod{72}$ and $(n-3) \not\equiv 0 \pmod{72}$

Of these factor pairs 8 and 9 stand out for having a difference of 1 between them, like our brackets, if we set $n = 11$ then this also solves our problem. 

Of the remaining factors there are no more clear pairs, however as we are working modulo 72 we must consider more complicated solutions.  

Equally negative factor pairs also multiply to 72 so -8 and -9 would be a solution. $-8 \equiv 64 \pmod{72}$ and $-9 \equiv 63 \pmod{72}$ allowing us to see another solution is when $n = 66$. 

From this we can now state all 4 possible values of $n$ 2,3,11,66.

If there is a more rigourous method to ensure all solutions are found please let me know, I think I'm forgetting a theorem here

This is alluded to here "In order to describe the solutions of a polynomial $f(x)$ over $\Z_n$ for any $n$, we need to find the roots of $f(x)$ over $\Z_{p^k} for prime powers $p^k$. We shall leave this for later." on this webpage https://crypto.stanford.edu/pbc/notes/numbertheory/poly.html

