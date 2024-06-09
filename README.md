# Machine-Learning-Tasks

Outlier detection is a crucial component of data analysis, aimed at identifying and addressing data points that significantly deviate from the majority of the dataset. These outliers, lying far from the bulk of the data, have the potential to skew statistical analyses, leading to biased findings and inaccurate interpretations. Detecting and appropriately handling outliers is vital for maintaining the integrity and reliability of data analysis.

There exist various methods for outlier detection, ranging from statistical techniques to visualization approaches. Statistical methods typically leverage measures of central tendency and dispersion, such as the mean, median, standard deviation, and interquartile range (IQR). These methods establish thresholds or ranges beyond which data points are flagged as outliers and either removed or treated accordingly.

Visualization techniques, including box plots, scatter plots, and histograms, offer graphical representations of the data that aid in outlier identification. For instance, box plots illustrate data distribution and highlight potential outliers as points outside the plot's whiskers. Scatter plots enable the visual examination of variable relationships, facilitating the identification of data points deviating from expected patterns.

The choice of outlier detection method should consider the data context and analysis objectives. While some methods suit normally distributed data, others prove robust against skewed distributions or outliers of varying magnitudes. Moreover, outlier detection is an iterative process, as removing outliers can influence subsequent analyses and may necessitate data reassessment.

Outlined below are common methods for outlier detection:

1. **Mean Function**: Calculate the mean and standard deviation of the 'price_per_sqft' column. Define a range around the mean (commonly ±3 standard deviations). Keep only the data points within this range.

2. **Percentile Method (IQR)**: Calculate the first quartile (Q1) and third quartile (Q3). Compute the interquartile range (IQR) as Q3 - Q1. Define lower bound as Q1 - 1.5 * IQR and upper bound as Q3 + 1.5 * IQR. Keep only the data points within this range.

3. **IQR (Interquartile Range) Method**: Similar to the percentile method but without recalculating quartiles, directly utilizing Q1 and Q3 to define outlier boundaries.

4. **Normal Distribution (Z-score)**:Calculate the z-score for each data point using the formula: Z-score =(X−mean)/standard deviation

Define a threshold (commonly 3). Keep only the data points with absolute z-scores less than the threshold.

5. **Z-score Method**: Same steps as Normal Distribution but without the absolute value.

Each method carries its strengths and limitations, necessitating careful consideration of the data characteristics and analytical requirements. By employing appropriate outlier detection techniques, analysts can enhance the accuracy and validity of their analyses, facilitating informed decision-making based on dependable data.

**Hypothesis testing** serves as a foundational statistical technique for drawing inferences about population parameters using sample data. It encompasses the formulation of competing hypotheses—the null hypothesis (H0) and the alternative hypothesis (Ha)—and their evaluation through empirical evidence. The null hypothesis posits no significant difference or effect, whereas the alternative hypothesis contends the presence of a significant difference or effect. By rigorously assessing the strength of evidence against the null hypothesis, hypothesis testing aids in determining the statistical significance of observed results across various domains, such as science, medicine, economics, and social sciences.

Key Steps in Hypothesis Testing:
1. **State the Hypotheses**: 
   - Null Hypothesis (H0): Represents the default assumption.
   - Alternative Hypothesis (Ha): Expresses the researcher's inquiry.

2. **Choose a Significance Level (α)**:
   - The significance level (α) denotes the probability of erroneously rejecting the null hypothesis when it holds true.

3. **Select the Appropriate Test Statistic**:
   - Tailoring the test statistic to the data type, sample size, and hypothesis under examination.

4. **Collect Data and Calculate the Test Statistic**:
   - Sample collection from the target population, followed by test statistic computation using the sample data.

5. **Determine the Critical Region or Critical Value**:
   - Identifying critical regions or values from the sampling distribution based on the chosen α and H0.

6. **Make a Decision**:
   - Comparing the computed test statistic against critical values or regions.
   - Rejecting H0 if the test statistic falls within the critical region; otherwise, failing to reject H0.

7. **Interpret the Results**:
   - Contextualizing the decision within the research question's framework.
   - Drawing conclusions regarding the population parameter.

8. **Conclusion**:
   - Stating the outcome, including whether H0 was rejected or retained.
   - Emphasizing that hypothesis testing provides evidence rather than absolute truth.

It's noteworthy that hypothesis testing does not offer definitive proof of H0's veracity or falsehood. Instead, it furnishes evidence supporting or refuting H0, contingent upon observed data and the chosen significance level. Furthermore, hypothesis testing constitutes just one facet of statistical inference, alongside estimation and prediction, in elucidating population characteristics from sample data.
