# Binomial Moments

This repo implements formulas for high-order moments of binomial distribution, discussed in the paper  "Handy formulas for Binomial Moments".

Here is how the sixth moment looks like, as a function of the probability parameter and the number of trials.

![image](https://github.com/maciejskorski/binomial_moments/assets/31315784/e7b67e97-9fec-4649-bbf1-a3e86a13e911)

And here are some first central moments:

| $d$   | $\mathbb{E}[S]^d, \quad S\sim\mathrm{Binom}(n,p)$ |
|-------|---------------------------------------------------|
| 1     | $p n$                                             |
| 2     | $p^{2} n^{\underline{2}} + p n$                   |
| 3     | $p^{3} n^{\underline{3}} + 3 p^{2} n^{\underline{2}} + p n$ |
| 4     | $p^{4} n^{\underline{4}} + 6 p^{3} n^{\underline{3}} + 7 p^{2} n^{\underline{2}} + p n$ |
| 5     | $p^{5} n^{\underline{5}} + 10 p^{4} n^{\underline{4}} + 25 p^{3} n^{\underline{3}} + 15 p^{2} n^{\underline{2}} + p n$ |
| 6     | $p^{6} n^{\underline{6}} + 15 p^{5} n^{\underline{5}} + 65 p^{4} n^{\underline{4}} + 90 p^{3} n^{\underline{3}} + 31 p^{2} n^{\underline{2}} + p n$ |
| 7     | $p^{7} n^{\underline{7}} + 21 p^{6} n^{\underline{6}} + 140 p^{5} n^{\underline{5}} + 350 p^{4} n^{\underline{4}} + 301 p^{3} n^{\underline{3}} + 63 p^{2} n^{\underline{2}} + p n$ |
| 8     | $p^{8} n^{\underline{8}} + 28 p^{7} n^{\underline{7}} + 266 p^{6} n^{\underline{6}} + 1050 p^{5} n^{\underline{5}} + 1701 p^{4} n^{\underline{4}} + 966 p^{3} n^{\underline{3}} + 127 p^{2} n^{\underline{2}} + p n$ |
| 9     | $p^{9} n^{\underline{9}} + 36 p^{8} n^{\underline{8}} + 462 p^{7} n^{\underline{7}} + 2646 p^{6} n^{\underline{6}} + 6951 p^{5} n^{\underline{5}} + 7770 p^{4} n^{\underline{4}} + 3025 p^{3} n^{\underline{3}} + 255 p^{2} n^{\underline{2}} + p n$ |
| 10    | $p^{10} n^{\underline{10}} + 45 p^{9} n^{\underline{9}} + 750 p^{8} n^{\underline{8}} + 5880 p^{7} n^{\underline{7}} + 22827 p^{6} n^{\underline{6}} + 42525 p^{5} n^{\underline{5}} + 34105 p^{4} n^{\underline{4}} + 9330 p^{3} n^{\underline{3}} + 511 p^{2} n^{\underline{2}} + p n$ |


