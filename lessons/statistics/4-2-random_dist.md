[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

    import nsfg
    import first
    import thinkstats2
    import thinkplot

    random_numbers = np.random.random(1000)
    pmf = thinkstats2.Pmf(random_numbers)
    thinkplot.Pmf(pmf)

    cdf = thinkstats2.Cdf(random_numbers)
    thinkplot.Cdf(cdf)
