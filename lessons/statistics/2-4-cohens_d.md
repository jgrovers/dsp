[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)


    resp = nsfg.ReadFemResp()
 
    pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')
    thinkplot.Pmf(pmf)
    thinkplot.Config(xlabel='Number of children', ylabel='PMF')
 
    biased = BiasPmf(pmf, label='biased')
    thinkplot.Pmf(biased)
    thinkplot.Config(xlabel='Number of children', ylabel='PMF')
 
    print("Actual mean:", pmf.Mean())
    print("Biased mean:", biased.Mean())
