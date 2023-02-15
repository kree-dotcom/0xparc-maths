3. Chinese Remainder Theorem 

i. Describe all integers such that $n \equiv 3 \pmod{5}$  and $n \equiv 6 \pmod{7}$ 

This is a basic example of applying Chinese remainder Theorem, while the shared notes did cover this I found it to be easier to follow this video https://www.youtube.com/watch?v=XoTEKjS61kI by Michael Penn.

We can apply CRT here because 5 and 7, our modulos, are coprime. 

Using the notation used in the video we have:

$N = 35$
$N_1 = 7$
$N_2 = 5$
$n_1 = 5$
$n_2 = 7$
$b_1 = 3$
$b_2 = 6$


We wish to solve $N_i x_i \equiv 1 \pmod{n_i}$  for i = 1,2

When i = 1:
$7x_1 \equiv 1 \pmod{5}$ 

Reduce $7 \pmod{5}$  to 2

$2x_1 \equiv 1  \pmod{5}$ 

Multiply by multiplicative inverse of 2 (mod 5), 3.

$x_1 \equiv 3  \pmod{5}$ 

When i = 2:
$5x_2 \equiv 1 \pmod{7}$ 

Multiply by multiplicative inverse of 5 (mod 7), also 3.

$x_2 \equiv 3 \pmod{7}$ 

Then we find $X = \sum x_iN_ib_i$

$X = 3 \times 7\times 3 + 3\times 5\times 6 = 63 + 90 = 153$

As $N = 35$ we reduce our answer modulo this

$X \equiv 13 \pmod{35}$ 

A quick (and incomplete) sanity check is to take some numbers, Y, that satisfy  $Y \equiv 13 \pmod{35}$  that and determine if they satisfy the original problem.

$13 \equiv 3  \pmod{5}$ 
$13 \equiv 6  \pmod{7}$ 

$48 \equiv 3  \pmod{5}$ 
$48 \equiv 6  \pmod{7}$  
 
 
ii. This problem is not as simple because 6 is not coprime to 8 and so we cannot apply the previous method straight away.

First we must find a way to get a system of modulos that are coprime. Looking at $n \equiv 5 \pmod(6)$ and $n \equiv 7 \pmod(8)$ we can deduce another modulo relationship for the greatest common divisor of 6 and 8, 24. 

If $n \equiv 5 \pmod(6)$ then $n \in (5,11,17,23) \pmod(24) 

and if $n \equiv 7 \pmod(8)$ then $n \in (7,15,23) \pmod(24) therefore we can see the only solution that solves both equations is $n \equiv 23 \pmod{24}$.

We now have the system of equations $n \equiv 23 \pmod{24}$ and $n \equiv 6 \pmod{7}$ here 24 and 7 are coprime so the same Chinese remainder theorem we used in part i can be applied again.

Using the same notation as before:

$N = 168$
$N_1 = 7$
$N_2 = 24$
$n_1 = 24$
$n_2 = 7$
$b_1 = 23$
$b_2 = 6$

We wish to solve $N_i x_i \equiv 1 \pmod{n_i}$  for i = 1,2

When i = 1: 
$7x_1 \equiv 1 \pmod{24}

7 is self-inverse modulo 24 so $x_1 \equiv 7 \pmod(24)$

When i =2:
$24x_2 \equiv 1 \pmod{7}$

Reduce 24 modulo 7.

$3x_2 \equiv 1 \pmod{7}$

The multiplicative inverse of 3 modulo 7 is 5 so we multiply by it.

$x_2 \equiv 5 \pmod{7}$

Then we find $X = \sum x_iN_ib_i$

$X = 7 \times 7 \times 23 + 5 \times 24 \times 6$

$X = 1847$

$1847 \equiv 167 \pmod{168}$ so $n \equiv 167 \pmod{168} is our answer.

Again we can check this against the original question

$167 \equiv 5 \pmod{6}$
$167 \equiv 6 \pmod{7}$
$167 \equiv 7 \pmod{8}$

