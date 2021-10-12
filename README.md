Communication Final Project
=======
This presentation will focus on the idea of regression and how to perform linear regression modeling in Python enviornment. In the beginning, we will introduce the principle of simple/multiple linear regression, followed by the packages we need to perform linear regression analysis in Python. Next, we will introduce different tests to determine the significance of each predictor variable and set dummies for categorical variables. In the end, we will demonstrate how to interpret those test results and finalize our model.

# Documents Included
[Data Source](https://github.com/summerzhang423/communication/blob/main/KelleyBlueBookData.csv)

[Code Reference](https://github.com/summerzhang423/communication/blob/main/communication_code.ipynb)

[Presentation Slides](https://github.com/summerzhang423/communication/blob/main/Communication%20Final.pdf) 


Packages
=======
[Pandas](https://pandas.pydata.org/about/) 

We will use Pandas package and its key data structure which is called the DataFrame to read data.

[Statsmodels](https://www.statsmodels.org/stable/index.html)

We will use Python’s statsmodels module to implement Ordinary Least Squares(OLS) method of linear regression and perform statistical tests.

Group Members
=======
[Yangzhou Tang](https://github.com/yangzhoutang)

[Isabella Zhai](https://github.com/isabellazhai)

# Hypothesis Test for Regression Slope
=======
The test focuses on the slope of the regression line Y = Β0 + Β1X, where Β0 is a constant, Β1 is the slope (also called the regression coefficient), X is the value of the independent variable, and Y is the value of the dependent variable.

If we find that the slope of the regression line is significantly different from zero, we will conclude that there is a significant relationship between the independent and dependent variables.

The test procedure consists of four steps: (1) state the hypotheses, (2) formulate an analysis plan, (3) analyze sample data, and (4) interpret results.

**(1) State the Hypotheses**
If there is a significant linear relationship between the independent variable X and the dependent variable Y, the slope will not equal zero.
Ho: Β1 = 0
Ha: Β1 ≠ 0

**(2) formulate an analysis plan**
The analysis plan describes how to use sample data to accept or reject the null hypothesis. 
In practice, we usually pick a significance level 0.05, althoug any number between 0 and 1 can be used.
Moreover, we pick a test method. In this example, we will use a linear regression t-test to determine whether the slope of the regression line differs significantly from zero.

**(3) analyze sample data**
In this example, we will use the package statsmodels introduced before, and this package will help us calculate the t-test results in a nice summary table. The summary tabl includes useful information such as the P-values and the coefficients. 

We are most interested in the P-value. The P-value is the probability of observing a sample statistic as extreme as the test statistic. If the p-value of one predictor is smaller than our chosen signifiance level, we can reject our null hypothesis and conclude that this specific predictor is significant to our model. 

**(4) interpret results**
Other than the P-value, the coefficients of predictors provide us information on how the x variable is changing with y. For a given coefficient of 100, we can say that for every unit increase in this predictor, we can expect 100 unit increas in our outcome y.

[Monty Xu](https://github.com/montyhsu)

[Summer Zhang](https://github.com/summerzhang423)
