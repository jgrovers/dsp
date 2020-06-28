[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

    # 5'10" = 70in
    # 6'1" = 73in
    cm_shortest = 70*2.54
    cm_tallest = 73*2.54

    shortest = dist.cdf(cm_shortest)
    tallest = dist.cdf(cm_tallest)
    print("""Amount of US men between 5'10" and 6'1":""",round((tallest-shortest)*100,2),"%")
