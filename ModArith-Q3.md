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

$X = 3*7*3 + 3*5*6 = 63 + 90 = 153$

As $N = 35$ we reduce our answer modulo this

$X \equiv 13 \pmod{35}$ 

A quick (and incomplete) sanity check is to take some numbers, Y, that satisfy  $Y \equiv 13 \pmod{35}$  that and determine if they satisfy the original problem.

$13 \equiv 3  \pmod{5}$ 
$13 \equiv 6  \pmod{7}$ 

$48 \equiv 3  \pmod{5}$ 
$48 \equiv 6  \pmod{7}$  
 
 
ii. This problem is not as simple because 6 is not coprime to 8 and so we cannot apply the previous method again.

