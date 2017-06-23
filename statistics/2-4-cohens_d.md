[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> >Cohen's d indicate that the mean difference between first born and others' weights is -0.089 standard deviations.
> The difference in mean for pregnancy length between the first born and others is 0.029 standard deviations.
>Both differences are quite small, but first born babies tend to be lighter and born later.
 
```python
from __future__ import print_function, division

import sys
import numpy as np
import thinkstats2

from collections import defaultdict

import thinkplot
import nsfg
import math

preg=nsfg.ReadFemPreg()
live=preg[preg.outcome==1]
irsts=live[live.birthord==1]
others=live[live.birthord!=1]
def CohenEffectSize(group1, group2):
    diff=group1.mean()-group2.mean()
    
    var1=group1.var()
    var2=group2.var()
    n1, n2=len(group1), len(group2)
    pooled_var=(n1*var1+n2*var2)/(n1+n2)
    d=diff/math.sqrt(pooled_var)
    return d

#Cohen's D for pregnancy length
CohenEffectSize(firsts.prglngth, others.prglngth)
#Cohen's D for totalwgt_lb
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
```
