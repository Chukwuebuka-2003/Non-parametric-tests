# Non-parametric-tests
My personal experimentation of non parametric test methods in python and data science

# Wilcoxon Signed-rank test
- It's often employed when the assumptions of parametric tests like the paired t-test are violated, such as when the data is not normally distributed or when the sample size is small.

## Theory:
- Assumptions: The Wilcoxon signed-rank test does not assume that the data follows a specific distribution, but it does require that the paired differences between the two samples are independent and that the data is at least ordinal.
- Null Hypothesis (H0): The null hypothesis states that there is no difference between the paired observations.
- Alternative Hypothesis (H1): The alternative hypothesis states that there is a difference between the paired observations.

### Procedure:
- Calculate the differences between paired observations.
- Discard any differences that equal zero.
- Rank the absolute values of the remaining differences from smallest to largest.
- Assign ranks, taking into account ties.
- Calculate the test statistic using the sum of the ranks of positive or negative differences (whichever is smaller).
- Compare the test statistic to a critical value from the Wilcoxon signed-rank distribution or use a significance level to determine statistical significance.

#### Interpretation:
- If the p-value is less than the chosen significance level, reject the null hypothesis and conclude that there is a statistically significant difference between the paired observations.
- If the p-value is greater than the chosen significance level, fail to reject the null hypothesis and conclude that there is not enough evidence to suggest a difference between the paired observations.

You can see the practical implementation of this statistic on the stat.ipynb notebook file
I'm open for suggestions and criticisms 
