[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> distribution looks quite uniform

```python
randomnumber=np.random.random(1000)

randomnumber_pmf = thinkstats2.Pmf(randomnumber, label='pmf')
randomnumber_cdf = thinkstats2.Cdf(randomnumber, label='cdf')
thinkplot.PrePlot(2)
thinkplot.Pmf(randomnumber_pmf)
thinkplot.Cdf(randomnumber_cdf)
thinkplot.Show(xlabel='random numbers', ylabel='PMF CDF')
```
