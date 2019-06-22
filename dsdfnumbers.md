---
layout: default
---

### Interesting Numbers 

Let _pq_ be the product of two distinct prime numbers whose [digit sum](https://en.wikipedia.org/wiki/Digit_sum) is equal to the difference of its factors. 

As an example, 14 is such a number: 1 + 4 = 7 - 2.

The first forty such numbers are:
```
14, 95, 527, 851, 1247, 3551, 4307, 8051, 14351, 26969, 30227, 37769, 64769, 87953, 152051, 163769, 199553, 202451, 256793, 275369, 341969, 455369, 1070969, 1095953, 1159673, 1232051, 1625369, 1702769, 2005007, 2081993, 2116769, 3674633, 4040051, 4397153, 4523873, 4600769, 4941473, 5075753, 5405369, 5630873
```

A csv file with all such numbers with prime factors less than a million can be found [here](./assets/valsMillion.csv)

Observations:
1. Given that 2 is the only even prime and the difference between 2 and the other primes grows much faster than the maximum possible digit sum of their product, it should be clear that 14 is the only even number with this property. For example, 53 - 2 = 51 is bigger than the largest possible digit sum for a 5-digit number, but 2 * 53 = 106, which is only a 3-digit number.

2. For products of prime numbers between 3 and 50 million, the numbers with this property have digit sums of 14, 32, 50, 68, 86, 104, or 122. _Question_: Is the digit sum of every such number 18 _n_ - 4, for some natural number _n_?
Examples of numbers with each of these digit sums: 
- 14: 95 = 5 * 19
- 32: 26969 = 149 * 181
- 50: 6593999 = 2543 * 2593
- 68: 399798869 = 19961 * 20029
- 86: 169987989767 = 412253 * 412339
- 104: 57779776889897 = 7601249 * 7601353
- 122: 1599996799997879 = 39999899 * 40000021
