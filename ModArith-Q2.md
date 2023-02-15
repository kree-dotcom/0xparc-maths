2. Cycles

i. What is the third-smallest positive value of $x$ for which $2^x \equiv 3 $ (mod 13)?


By Lagrange's theorem as the order of a element in a group must divide the order of the group we can tell that
the order of the element 2 must divide the order of $\mathds{Z}_{13}$ therefore it must be 1 or 13. It is trivially not 1 and so 2 must be a generator of $\mathds{Z}_{13}$ as it is also order 13. 


Our first step then is to find the first-smallest positive value where 

$2^x \equiv 3 $ (mod 13).

We can see this occurs when $x = 4$. Then because 2 is cyclic and we know that $2^{12} \equiv 1 $ (mod 13) by Fermat's little theorem we can deduce the second-smallest and third-smallest positive values as such:

$2^4 * 2^{12} \equiv 3 * 1 \equiv 2^{16}$ (mod 13)


$2^4 * 2^{12} * 2^{12}  \equiv 3 * 1 * 1\equiv 2^{28}$ (mod 13)

And so the answer is $ x = 28$.

ii. What is the fourth-smallest positive value of $x$ for which $2^x \equiv 8 $ (mod 101)?

In the last question because the order of the group was small a brute-force solution would also be viable, here we use the same approach as above as a brute-force solution becomes time consuming. The previous answer explains the logic behind the following steps.

Our first step is to find the first-smallest positive value where 

$2^x \equiv 8 $ (mod 101).

Clearly this is $ x = 3$ 

Then using Fermat's little theorem 

$2^{100} \equiv 1 $ (mod 101).


Hence 


$2^3 * 2^{100} * 2^{100} * 2^{100} \equiv 8 * 1 * 1 * 1 \equiv 8 \equiv 2^{303}$ (mod 101).

The answer is $ x = 303$.
