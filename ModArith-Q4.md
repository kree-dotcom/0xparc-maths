4. Modular Inverses

i. $5n + 7 \equiv 2 \pmod{13}$

subtract 7

$5n \equiv -5 \equiv 8 \pmod{13}$

Multiply by multiplicative inverse of $5  \pmod{13}$, 8. 
This can quickly be found by recognising that $5 \times 5 \equiv 25 \equiv -1 \pmod{13}$
Therefore $5 \times -5 \equiv 1 \pmod{13}$ and $-5 \equiv 8 \pmod{13}$

$n \equiv 64 \equiv 12 \pmod{13}$

ii. $3n + 9 \equiv 4 \pmod{12}$

This has no solution because reduced it becomes $3n \equiv 7 \pmod{12}$ and 3 and 12 are not coprime but 7 is not divisible by their factor 3.

iii. $3n + 9 \equiv 3 \pmod{12}$

Here there is a common factor of 3 so we divide by it to gain:

$n +3 \equiv 1 \pmod{4}$

$n \equiv 2 \pmod{4}$

However as the original problem was $\pmod{12}$ we must state all solutions so when $n \in (2,6,10)$

iv. $19n \equiv 1 \pmod{257}$ 19,1 and 257 are all prime so the problem cannot be reduced.

We wish to find the multiplicative inverse of $19 \pmod{257}$, 230. 

You can find this using the extended Euclidean algorithm.

It is also possible to find the answer using a special multiplicative inverse calculator that you can find online if you are short of time.

The extended Euclidean algorithm is explained here http://www-math.ucdenver.edu/~wcherowi/courses/m5410/exeucalg.html

For our calculation we find the multiplicative inverse of 19 modulo 257 as follows:

$257 = 13 \times 19 + 10$

$19 = 1 \times 10 + 9$

$10 = 1 \times 9 + 1$

Now that we have found a remainder 1 we rearrange each equation to make the remainder the subject

$10 = 257 - 13 \times 19$
$9 = 19 - 1 \times 10$
$1 = 10 - 1 \times 9$

Now we substitute each remainder into the bottom equation.

$1 = 10 - 1 \times (19 - 1 \times 10) = 2 \times 10 - 19$

$1 = 2 \times (257 - 13 \times 19) - 19 = 2 \times 257 - 27 \times 19 $

Therefore multiplying 19 -27 times will give us the multiplicative inverse of 19 modulo 257 and $-27 \equiv 230 \pmod{257}$

Multiplying our original equation by this gives us the answer $n \equiv 230 \pmod{257}$ 
