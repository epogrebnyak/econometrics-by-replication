Ordinary least squares, OLS
---------------------------

OLS is at the core of econometrics curriculum, it is easily derived and
highly practical to familiarise a learner with regression possibilites
and limitations.

The usual way to teach OLS is to present assumptions and show how to deal
with their violations as indicated below in a review chart from Kennedy's
textbook.


.. image:: .\_static\peter_kennedy_on_ols.png


Math:

:math:`Y = \beta X + \epsilon`, :math:`\epsilon` is iid, normal with finite variance.

Common steps: 

1. specify model: select explanatory variables, transform them if needed 
2. estimate coefficients 
3. elaborate on model quality (the hardest part) 
4. go to 1 if needed 
5. know what model *does not* show (next hardeer part)

What may go wrong: 

- residuals are not random 
- variables are cointegrated 
- multicollinearity in regressors 
- residuals depend on x (heteroscedasticity) 
- inference is not causality 
- wrong signs, insignificant coefficients 
- variable normalisation was not described

Discussion: 

- why sum of squares as a loss function? 
- connections to bayesian estimation
- is R2 useful or dangerous?

Replication examples: 

- https://www.kaggle.com/nicapotato/in-depth-simple-linear-regression

Implementations:

- [lm function in R](https://github.com/wch/r-source/blob/0f07757ad10ca31251b28a2c332812e63c0acf38/src/library/stats/R/lm.R) 
- [OLS class in python statsmodels](https://github.com/statsmodels/statsmodels/blob/master/statsmodels/regression/linear_model.py)
- [python scypi least squares](https://github.com/scipy/scipy/blob/v1.1.0/scipy/linalg/basic.py#L1048-L1265)
- julia [Alistair](https://github.com/giob1994/Alistair.jl), GLM.jl, Regression.jl

Links (preliminary):

-  https://stats.stackexchange.com/questions/296514/is-ols-estimator-the-only-blue-estimator
-  https://cran.r-project.org/doc/contrib/Faraway-PRA.pdf
-  https://github.com/marcoalt/Regression-parameter-estimates
-  https://blog.minitab.com/blog/how-to-choose-the-best-regression-model
-  https://towardsdatascience.com/simple-linear-regression-2421076a5892
-  https://papers.ssrn.com/sol3/papers.cfm?abstract\_id=1736184
-  https://cfss.uchicago.edu/persp012\_regression\_diagnostics.html
-  https://stats.stackexchange.com/questions/218156/what-are-some-of-the-most-common-misconceptions-about-linear-regression
-  https://pdfs.semanticscholar.org/a410/ec58bd5ff80a4e7978955ab11d096af6d138.pdf
-  `COMMON MISTEAKS MISTAKES IN USING STATISTICS: Spotting and Avoiding
   Them <https://web.ma.utexas.edu/users/mks/statmistakes/StatisticsMistakes.html>`__
-  http://www2.sas.com/proceedings/sugi22/STATS/PAPER267.PDF
-  https://towardsdatascience.com/simple-linear-regression-2421076a5892
-  http://jeromyanglim.blogspot.com/2013/12/using-r-to-replicate-common-spss.html
-  https://stat.hevra.haifa.ac.il/~gweiss/courses/Forecasting/CarPricesAnalysis.pdf
-  http://www.nrcresearchpress.com/doi/10.1139/f73-072#.W-SvWuK\_Pcs
-  https://www.nejm.org/doi/full/10.1056/NEJM198512263132604
-  https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2992018/ - medicine,
   nice!
-  http://replication.uni-goettingen.de/wiki/index.php/Ordinary\_least\_squares\_(OLS)
   - list of replications
-  https://stats.stackexchange.com/questions/211707/replicating-a-linear-regression-example-from-hastie-tibshirani-and-friedman
   (replication from Hastie)

Intuitive learning for OLS 

- `Stackoverflow hot
topics <https://stats.stackexchange.com/questions/tagged/linear-model?sort=votes&pageSize=15>`__
- `In Depth: Linear
Regression <https://jakevdp.github.io/PythonDataScienceHandbook/05.06-linear-regression.html>`__
- Stachurski math intro:
  - `TOC <https://mitpress.mit.edu/sites/default/files/Stachurski_final_TOC.pdf>`__
  - `slides <https://github.com/jstac/econometric_theory_slides>`__ 
- https://lectures.quantecon.org/py/ols.html 
- http://www.statsmodels.org/stable/examples/index.html#regression 
- https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.lstsq.html
- https://stats.stackexchange.com/questions/1829/what-algorithm-is-used-in-linear-regression
