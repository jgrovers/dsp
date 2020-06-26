[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)


    def cohens_d(firsts, others):
        mean_firsts = firsts.totalwgt_lb.mean()
        mean_others = others.totalwgt_lb.mean()
        diff = mean_firsts - mean_others
    
        variance_firsts = firsts.totalwgt_lb.var()
        variance_others = others.totalwgt_lb.var()
    
        n_firsts = len(firsts)
        n_others = len(others)
    
        pooled_variance = (n_firsts * variance_firsts + n_others * variance_others)
        d = diff / math.sqrt(pooled_variance)
    
        print("Cohen's d:",d)
