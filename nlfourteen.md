---
layout: default
mathjax: true
---

### Numbers Like Fourteen

The number \\( 14 \\) has the property that the [sum of its digits](https://en.wikipedia.org/wiki/Digit_sum) is equal to the difference of its prime factors. That is, \\( 14 = 2 * 7 \\) and \\( 1 + 4 = 7 - 2 \\).

I noticed this many years ago, but until recently, I never took the time to look for other such numbers. As it turns out, there are quite a few. (_Infinitely many?_)

Let's say that a number is _like fourteen_ if it is the [product of two primes](https://en.wikipedia.org/wiki/Semiprime) and its digit sum is equal to the difference of its prime factors. The first fifty numbers like fourteen are:
```
14, 95, 527, 851, 1247, 3551, 4307, 8051, 14351, 26969, 30227, 37769, 64769, 87953, 152051, 163769, 199553, 202451, 256793, 275369, 341969, 455369, 1070969, 1095953, 1159673, 1232051, 1625369, 1702769, 2005007, 2081993, 2116769, 3674633, 4040051, 4397153, 4523873, 4600769, 4941473, 5075753, 5405369, 5630873, 6036593, 6593999, 7144673, 7305953, 7935233, 9941153, 9997619, 10304051, 10477913, 11390369
```

The first 1000 numbers like are fourteen can be downloaded [here](./assets/first1000.txt). This list and the observations below were made with variations of the python scripts found [here](https://github.com/jebeyer/nlfourteen-py).

**Observations**:

1. Given that \\( 2 \\) is the only even prime and \\( p - 2 \\) grows much faster than the digit sum of \\( 2p \\), it is clear that \\( 14 \\) is the only even number like fourteen.

2. Other than \\( 14 \\), every number like fourteen that I have found has a digit sum of \\( 18n - 4 \\) for some natural number \\( n \\). (_Is this true for all odd numbers like fourteen?_)

    digit sum  | product           | factor a  | factor b
    ---------- | ----------------- | --------- | ----------
    14         | 95                | 5         | 19
    32         | 26969             | 149       | 181
    50         | 6593999           | 2543      | 2593
    68         | 399798869         | 19961     | 20029
    86         | 169987989767      | 412253    | 412339
    104        | 57779776889897    | 7601249   | 7601353
    122        | 1599996799997879  | 39999899  | 40000021
    
3. It is possible for multiple numbers like fourteen to share a factor. That is, there are prime numbers \\( a < b < c \\) such that either \\( ab \\) and \\( ac \\) are both like fourteen or \\( ac \\) and \\( bc \\) are both like fourteen. Here is an example:

    product      | factor a    | factor b
    ------------ | ----------- | -----------
    25449182159  | 159503      | **159553**
    25452054113  | **159521**  | **159553**
    25454925491  | **159521**  | 159571
    25457796869  | **159521**  | **159589**
    25460669471  | 159539      | **159589**

4. There are numbers like fourteen with nested factors. That is, there are prime numbers \\( a < b < c < d \\) such that \\( ad \\) and \\( bc \\) are both like fourteen. Here is one example:

    product  | factor a  | factor b
    -------- | --------- | ---------
    199553   | 431       | 463
    202451   | 443       | 457

5. I haven't found any prime numbers \\( x < y < z \\) such that \\( xy \\) and \\( yz \\) are both like fourteen. (_Do such numbers exist?_)

6. For every odd number like fourteen that I have found, the sum of the factors is a multiple of \\( 6 \\). If we write the factors as \\( a < b \\), then combined with observation 2 above, \\( a = 6m - 1 \\) and \\( b = 6n + 1 \\) for some \\( m,n \in \mathbb{N} \\). If this is true for all odd numbers like fourteen, that would mean that the answer to the question in observation 5 is no.

7. Not every combination of primes fitting the above patterns generates a number like fourteen. For example, \\( 2867 = 47 * 61 \\), and \\( 2867 \\) is not like fourteen. 

---

_last updated: 2019-06-28_



