[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> resp = nsfg.ReadFemResp()

>> pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

>> biased = BiasPmf(pmf, label='biased')
thinkplot.Pmf(biased)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

>> print("Actual mean:", pmf.Mean())

>> print("Biased mean:", biased.Mean())
