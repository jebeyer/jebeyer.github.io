---
layout: default
---

### DSDF Numbers 

Let _pq_ be the product of two distinct prime numbers whose [digit sum](https://en.wikipedia.org/wiki/Digit_sum) is equal to the difference of its factors. Until I think of a better name, we can call _pq_ a **DSDF number**.

For example, 14 is a DSDF number: 1 + 4 = 7 - 2.

The first forty DSDF numbers are:
```
14, 95, 527, 851, 1247, 3551, 4307, 8051, 14351, 26969, 30227, 37769, 64769, 87953, 152051, 163769, 199553, 202451, 256793, 275369, 341969, 455369, 1070969, 1095953, 1159673, 1232051, 1625369, 1702769, 2005007, 2081993, 2116769, 3674633, 4040051, 4397153, 4523873, 4600769, 4941473, 5075753, 5405369, 5630873
```

A csv file with all DSDF numbers with prime factors less than a million can be found [here](./assets/valsMillion.csv)

Observations:
1. Given that 2 is the only even prime and the difference between 2 and the other primes grows much faster than the maximum possible digit sum of their product, it should be clear that 14 is the only even DSDF number.

2. For products of prime numbers between 3 and 50 million, the DSDF numbers have digit sums of 14, 32, 50, 68, 86, 104, or 122. _Question_: Is the digit sum of every DSDF number 18_n_ - 4 for some natural number _n_?

Examples of DSDF numbers with each of these digit sums: 
digit sum  | product | factor a | factor b
---|---|---|---
14 | 95 | 5 | 19
32 | 26969 | 149 | 181
50 | 6593999 | 2543 | 2593
68 | 399798869 | 19961 | 20029
86 | 169987989767 | 412253 | 412339
104 | 57779776889897 | 7601249 | 7601353
122 | 1599996799997879 | 39999899 | 40000021

3. It is possible for multiple DSDF numbers to share a factor. That is, there are prime numbers _a < b < c_ such that either _ab_ and _ac_ are DSDF numbers or _ac_ and _bc_ are DSDF numbers. Here is one interesting set of numbers that share factors:

product     | factor a | factor b
----------- | -------- | -----------
25449182159 | 159503   | _159553_
25452054113 | _159521_ | _159553_
25454925491 | _159521_ | 159571
25457796869 | _159521_ | _159589_
25460669471 | 159539   | _159589_

4. There are DSDF numbers with nested factors. That is, DSDF numbers _xw_ and _yz_ with _x < y < z < w_. Here is one example:
product | factor a | factor b
---|---|---
199553 | 431 | 463
202451 | 443 | 457

5. I have not found an instance of DSDF numbers _xy_ and _yz_ such that _x < y < z_. _Question_: Do such numbers exist?
