Logistic regression model explaining the willingness to share data and scripts.

Explaining variables:

- sexmale: 0 = female, 1 = male
- age in years
- open: openness (big five)
- cons: conscientiousness (big five)
- extr: extraversion (big five)
- agre: agreeableness (big five)
- neur: neuroticism (big five)

-----

```
Call:
glm(formula = will_share ~ sex + age + open + cons + extr + agre + 
    neur, family = "binomial", data = data)

Deviance Residuals: 
    Min       1Q   Median       3Q      Max  
-2.3492   0.4241   0.5303   0.6361   1.1986  

Coefficients:
            Estimate Std. Error z value Pr(>|z|)   
(Intercept)  1.81216    1.45559   1.245  0.21314   
sexmale     -0.28170    0.31666  -0.890  0.37368   
age         -0.02420    0.01243  -1.947  0.05152 . 
open         0.43856    0.15615   2.809  0.00497 **
cons        -0.17777    0.17515  -1.015  0.31011   
extr         0.12908    0.11926   1.082  0.27908   
agre        -0.15782    0.16186  -0.975  0.32953   
neur        -0.04137    0.09268  -0.446  0.65533   
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

(Dispersion parameter for binomial family taken to be 1)

    Null deviance: 346.61  on 376  degrees of freedom
Residual deviance: 329.49  on 369  degrees of freedom
  (290 observations deleted due to missingness)
AIC: 345.49

Number of Fisher Scoring iterations: 4
```
