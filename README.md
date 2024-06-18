[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Naereen/badges)

# Binomial Moments

This repo implements formulas for high-order moments of binomial distribution, discussed in the paper  "Handy formulas for Binomial Moments".

Here is how the sixth moment looks like, as a function of the probability parameter and the number of trials.

![image](https://github.com/maciejskorski/binomial_moments/assets/31315784/e7b67e97-9fec-4649-bbf1-a3e86a13e911)

And here are some first central moments, with $q=1-p,\sigma^2=pq$:

| $d$ | $\mathbb{E}[(S-\mathbb{E}[S])^d],\quad S\sim\mathrm{Binom}(n,p)$ |
|-----|------------------------------------------------------------------|
| 2   | $n \sigma^{2}$                                                   |
| 3   | $n \sigma^{2} \left(- 2 p + 1\right)$                            |
| 4   | $3 n^{2} \sigma^{4} + n \left(- 6 \sigma^{4} + \sigma^{2}\right)$ |
| 5   | $\left(- 2 p + 1\right) \left(10 n^{2} \sigma^{4} + n \left(- 12 \sigma^{4} + \sigma^{2}\right)\right)$ |
| 6   | $15 n^{3} \sigma^{6} + n^{2} \left(- 130 \sigma^{6} + 25 \sigma^{4}\right) + n \left(120 \sigma^{6} - 30 \sigma^{4} + \sigma^{2}\right)$ |
| 7   | $\left(- 2 p + 1\right) \left(105 n^{3} \sigma^{6} + n^{2} \left(- 462 \sigma^{6} + 56 \sigma^{4}\right) + n \left(360 \sigma^{6} - 60 \sigma^{4} + \sigma^{2}\right)\right)$ |
| 8   | $105 n^{4} \sigma^{8} + n^{3} \left(- 2380 \sigma^{8} + 490 \sigma^{6}\right) + n^{2} \left(7308 \sigma^{8} - 2156 \sigma^{6} + 119 \sigma^{4}\right) + n \left(- 5040 \sigma^{8} + 1680 \sigma^{6} - 126 \sigma^{4} + \sigma^{2}\right)$ |
| 9   | $\left(- 2 p + 1\right) \left(1260 n^{4} \sigma^{8} + n^{3} \left(- 13216 \sigma^{8} + 1918 \sigma^{6}\right) + n^{2} \left(32112 \sigma^{8} - 6948 \sigma^{6} + 246 \sigma^{4}\right) + n \left(- 20160 \sigma^{8} + 5040 \sigma^{6} - 252 \sigma^{4} + \sigma^{2}\right)\right)$ |
| 10  | $945 n^{5} \sigma^{10} + n^{4} \left(- 44100 \sigma^{10} + 9450 \sigma^{8}\right) + n^{3} \left(303660 \sigma^{10} - 99120 \sigma^{8} + 6825 \sigma^{6}\right) + n^{2} \left(- 623376 \sigma^{10} + 240840 \sigma^{8} - 24438 \sigma^{6} + 501 \sigma^{4}\right) + n \left(362880 \sigma^{10} - 151200 \sigma^{8} + 17640 \sigma^{6} - 510 \sigma^{4} + \sigma^{2}\right)$ |




These formulas can be used to obtain skewness and kurtosis:

|                 |                                             |
|-----------------|---------------------------------------------|
| skewness        | $\frac{1-2p}{\sqrt{npq}}$                   |
| excess kurtosis | $\frac{1-6pq}{npq}$                         |

