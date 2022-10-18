# Correlation

In statistics correlation is any statistical relationship, causal or not between two random variables.
The ranges of correlation varies from -1 to 1.

# Machine learning
We say that a machine is learning when it improves its performance,without being explicitly programmed to do so, after making observations about the world.
Depending on the feedback that accompany the input there is a distinction between the types of learning:
- ## Supervised learning:
    Data contains inputs and outputs. The machine has to learn what is the hypothesis $h$ that maps inputs to outputs. Depending on the output type the problems differentiate in:
    - ### Classification: 
        When the output is a finite set of values.
    - ### Regression:
        When the output is a number.

# One-Hot encoding
When dealing with categorical attributes, is helpful to transform them into n districnt boolean attributes, i.e if we have this attributes:
- Cloudy
- Sunny 
- Rainy 
We add each value as a column and for every row activate only the correct value.

# Feature scaling

- ## Min-Max scaling :
    Values are shifted and rescaled so that they end up rangin between 0 and 1. This is oftern performed subracting the minimum value and dividing by the maximum minus the minimum.
    $$\frac{Value-min}{max-min}$$

- ## Standardization:
    First subtracts the mean and then divides by the standard deviation resulting in values having zero mean and unit variance.
    $$\frac{Value-\mu}{\sigma}$$

Standardization doesn't map the values between 0 and 1 so it might still be problematic for some algorithms, but in return standardization is less more aftected by the outliers. 