[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> percentage is 0.34209 for males

```python
import scipy.stats
height_m = scipy.stats.norm(loc=178, scale=7.7)
low=height_m.cdf(177.8)
high=height_m.cdf(185.4)
high-low
```
