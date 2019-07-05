# [Analyzing A/B Test Results](https://alfred-kctang.github.io/Analyzing-AB-Test-Results-Project/)

## Table of Contents

* [Introduction](#intro)
* [Statistical Methods Used](#statMethodsUsed)
* [Conclusion](#conclusion)
* [License](#license)

## Introduction

A/B tests are very commonly performed by data analysts and data scientists. In this project, I was trying to run A/B tests with two approaches, (1) hypothesis testing and (2) logistic regression, and to interpret the results for an imaginery e-commerce company. The company has developed a new web page in order to try to increase the number of viewers who "convert", i.e. the number of viewers who decide to pay for the company's product. My goal is to help the company understand if it should implement this new page, keep the old page, or perhaps run the experiment longer to make a decision.

## Statistical Methods Used

- Probability
- Hypothesis Testing
- Bootstrapping
- A/B Testing
- Z-test
- Logistic Regression

## Conclusion

In the first approach with hypothesis testing technique, I performed an A/B testing along with simulations by bootstrapping to see whether the new page leads to higher conversion rate, i.e. the proportion of viewers who decide to pay for a given product, than its old counterpart, and concluded that there is no statistically significant difference between the old and new pages. I then conducted a z-test to confirm the above results.

In the second approach with logistic regression technique, I performed another A/B testing to test whether there is any linear relationship between a binary variable, whether a given viewer received the old or new page, and the response variable, the probability of converting. Afterwards, I added another categorical variable, which indicates the country that a viewer lives in, into the logistic regression model, and then added the interaction terms between the above-mentioned binary variable and this categorical variable to see whether the way the binary variable is related to the response variable, i.e. the probability of converting, depends on this categorical variable.

Though the ways that the two A/B tests were conducted are entirely different, both of them lead to the same conclusion: there is no statistically significant difference in conversion rates between those viewers who receive the new page and those who receive the old one. Based on this findings, I would recommend the company to keep the old page.

## License

This repository is covered under the [MIT License](https://choosealicense.com/licenses/mit/).
