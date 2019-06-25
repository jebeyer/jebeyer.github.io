---
layout: default
mathjax: true
---

### Numbers Like Fourteen

The number \\( 14 \\) has the interesting property that its [digit sum](https://en.wikipedia.org/wiki/Digit_sum) is equal to the difference of its prime factors. That is, \\( 14 = 7 * 2 \\) and \\( 1 + 4 = 7 - 2 \\).

I noticed this many years ago, but until recently, I never took the time to look for other such numbers. As it turns out, there are quite a few. (_Infinitely many?_)

Let's say that a number is _like fourteen_ if it is the product of two distinct primes and its digit sum is equal to the difference of its prime factors. The first forty numbers like fourteen (NLF) are:
```
14, 95, 527, 851, 1247, 3551, 4307, 8051, 14351, 26969, 30227, 37769, 64769, 87953, 152051, 163769, 199553, 202451, 256793, 275369, 341969, 455369, 1070969, 1095953, 1159673, 1232051, 1625369, 1702769, 2005007, 2081993, 2116769, 3674633, 4040051, 4397153, 4523873, 4600769, 4941473, 5075753, 5405369, 5630873
```

**Observations**:

1. Given that \\( 2 \\) is the only even prime and \\( p - 2 \\) grows much faster than the digit sum of \\( 2p \\), it is clear that \\( 14 \\) is the only even NLF.

2. Other than \\( 14 \\), every NLF that I have found has a digit sum of \\( 18n - 4 \\) for some natural number \\( n \\). (_Is this true for all NLF?_)

    digit sum | product          | factor a | factor b
    --------- | ---------------- | -------- | ---------
    14        | 95               | 5        | 19
    32        | 26969            | 149      | 181
    50        | 6593999          | 2543     | 2593
    68        | 399798869        | 19961    | 20029
    86        | 169987989767     | 412253   | 412339
    104       | 57779776889897   | 7601249  | 7601353
    122       | 1599996799997879 | 39999899 | 40000021
    
3. It is possible for multiple NLF to share a factor. That is, there are prime numbers \\( a < b < c \\) such that either \\( ab \\) and \\( ac \\) are both NLF or \\( ac \\) and \\( bc \\) are both NLF. Here is an example:

    product     | factor a | factor b
    ----------- | -------- | -----------
    25449182159 | 159503   | _159553_
    25452054113 | _159521_ | _159553_
    25454925491 | _159521_ | 159571
    25457796869 | _159521_ | _159589_
    25460669471 | 159539   | _159589_

4. There are NLF with nested factors. That is, there are prime numbers \\( a < b < c < d \\) such that \\( ad \\) and \\( bc \\) are both NLF. Here is one example:

    product | factor a | factor b
    ------- | -------- | --------
    199553  | 431      | 463
    202451  | 443      | 457

5. I haven't found any prime numbers \\( x < y < z \\) such that \\( xy \\) and \\( yz \\) are both NLF. (_Do such numbers exist?_)


