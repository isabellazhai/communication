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

The test focuses on the slope of the regression line Y = Β0 + Β1X, where Β0 is a constant, Β1 is the slope (also called the regression coefficient), X is the value of the independent variable, and Y is the value of the dependent variable.

If we find that the slope of the regression line is significantly different from zero, we will conclude that there is a significant relationship between the independent and dependent variables.

The test procedure consists of four steps: (1) state the hypotheses, (2) formulate an analysis plan, (3) analyze sample data, and (4) interpret results.

1) 
If there is a significant linear relationship between the independent variable X and the dependent variable Y, the slope will not equal zero.
Ho: Β1 = 0
Ha: Β1 ≠ 0

2) 
Significance level: Often, we choose significance levels equal to 0.01, 0.05, or 0.10; but any value between 0 and 1 can be used.
Test method: Use a linear regression t-test to determine whether the slope of the regression line differs significantly from zero.

3)
In this step, we either calculate the test statistics and the p-value by hand, or we can seek help from programming tools.

4)
In the last part, we interpret the test results, compare the p-value with the chosen signficance level, and decide which predictors are significant to our model.


![alt text](https://www.facebook.com/photo/?fbid=2629070530571871&set=a.1081858695293070)

The statsmodels package provides a nice summary table of the test results. Here, we can check the p-value of each predictors we are interested in and see how the response variable is changing with every unit change of a specific predictor. 

[Monty Xu](https://github.com/montyhsu)

[Summer Zhang](https://github.com/summerzhang423)
