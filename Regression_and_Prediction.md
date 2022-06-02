https://www.oreilly.com/library/view/practical-statistics-for/9781492072935/ch04.html

# Regression and Prediction

```
KEY IDEAS
The regression equation models the relationship between a response variable Y and a predictor variable X as a line.

A regression model yields fitted values and residuals—predictions of the response and the errors of the predictions.

Regression models are typically fit by the method of least squares.

Regression is used both for prediction and explanation.
```

```
KEY IDEAS
Multiple linear regression models the relationship between a response variable Y and multiple predictor variables X1,...,Xp.

The most important metrics to evaluate a model are root mean squared error (RMSE) and R-squared (R2).

The standard error of the coefficients can be used to measure the reliability of a variable’s contribution to a model.

Stepwise regression is a way to automatically determine which variables should be included in the model.

Weighted regression is used to give certain records more or less weight in fitting the equation.
```

```
KEY IDEAS
Extrapolation beyond the range of the data can lead to error.

Confidence intervals quantify uncertainty around regression coefficients.

Prediction intervals quantify uncertainty in individual predictions.

Most software, R included, will produce prediction and confidence intervals in default or specified output, using formulas.

The bootstrap can also be used to produce prediction and confidence intervals; the interpretation and idea are the same.
```

```
KEY IDEAS
Factor variables need to be converted into numeric variables for use in a regression.

The most common method to encode a factor variable with P distinct values is to represent them using P – 1 dummy variables.

A factor variable with many levels, even in very big data sets, may need to be consolidated into a variable with fewer levels.

Some factors have levels that are ordered and can be represented as a single numeric variable.
```

```
KEY IDEAS
Because of correlation between predictors, care must be taken in the interpretation of the coefficients in multiple linear regression.

Multicollinearity can cause numerical instability in fitting the regression equation.

A confounding variable is an important predictor that is omitted from a model and can lead to a regression equation with spurious relationships.

An interaction term between two variables is needed if the relationship between the variables and the response is interdependent.
```

```
KEY IDEAS
While outliers can cause problems for small data sets, the primary interest with outliers is to identify problems with the data, or locate anomalies.

Single records (including regression outliers) can have a big influence on a regression equation with small data, but this effect washes out in big data.

If the regression model is used for formal inference (p-values and the like), then certain assumptions about the distribution of the residuals should be checked. In general, however, the distribution of residuals is not critical in data science.

The partial residuals plot can be used to qualitatively assess the fit for each regression term, possibly leading to alternative model specification.
```

```
KEY IDEAS
Outliers in a regression are records with a large residual.

Multicollinearity can cause numerical instability in fitting the regression equation.

A confounding variable is an important predictor that is omitted from a model and can lead to a regression equation with spurious relationships.

An interaction term between two variables is needed if the effect of one variable depends on the level or magnitude of the other.

Polynomial regression can fit nonlinear relationships between predictors and the outcome variable.

Splines are series of polynomial segments strung together, joining at knots.

We can automate the process of specifying the knots in splines using generalized additive models (GAM).
```

Summary
Perhaps no other statistical method has seen greater use over the years than regression—the process of establishing a relationship between multiple predictor variables and an outcome variable. The fundamental form is linear: each predictor variable has a coefficient that describes a linear relationship between the predictor and the outcome. More advanced forms of regression, such as polynomial and spline regression, permit the relationship to be nonlinear. In classical statistics, the emphasis is on finding a good fit to the observed data to explain or describe some phenomenon, and the strength of this fit is how traditional in-sample metrics are used to assess the model. In data science, by contrast, the goal is typically to predict values for new data, so metrics based on predictive accuracy for out-of-sample data are used. Variable selection methods are used to reduce dimensionality and create more compact models.
