# Descriptive-Statistics
### An easy descriptive statistics approach to summarize the numeric and categoric data variables for every Exploratory Data Analysis process.

This notebook presents the descriptive statistics of the numerical and categorical variables through the measures of central tendency and measures of spread.

Statistics is divided into two major areas:
- Descriptive statistics: describe and summarize data;
- Inferential statistics: methods for using sample data to make general conclusions (inferences) about populations.

This tutorial focuses on descriptive statistics of both numerical and categorical variables and is divided into two parts:
- Measures of central tendency
- Measures of spread

Also named **Univariate Analysis** (one feature analysis at a time), descriptive statistics, in short, help describe and understand the features of a specific dataset, by giving short numeric summaries about the sample and measures of the data. Descriptive statistics are mere exploration as they **do not** allows us to make conclusions beyond the data we have analysed or reach conclusions regarding any hypotheses we might have made.Numerical and categorical variables, as we will see shortly, have different descriptive statistics approaches.

Let’s review the type of variables:
- Numerical continuous: The values are not countable and have an infinite number of possibilities (Someone’s age: 25 years, 4 days, 11 hours, 24 minutes, 5 seconds and so on to the infinite)
- Numerical discrete: The values are countable and have an finite number of possibilities (It is impossible to count 27.52 countries in the EU)
- Categorical ordinal: There is an order implied in the levels (January comes always before February and after December)
- Categorical nominal: There is no order implied in the levels (Female/male, or the wind direction: north, south, east, west)

## **Numerical variables**
- Measures of central tendency: Mean, median
- Measures of spread: Standard deviation, variance, percentiles, maximum, minimum, skewness, kurtosis
- Others: Size, unique, number of uniques

One approach to display the data is through a boxplot. It gives you the 5-basic-stats, such as the minimum, the 1st quartile (25th percentile), the median, the 3rd quartile (75th percentile), and the maximum.

## **Categorical variables**
- Measures of central tendency: Mode (most common)
- Measures of spread: Number of uniques
- Others: Size, % Highest unique

Understanding:

### **Measures of central tendency**
- Mean (average): The total sum of values divided by the total observations. The mean is highly sensitive to the outliers
- Median (center value): The total count of an ordered sequence of numbers divided by 2. The median is not affected by the outliers
- Mode (most common): The values most frequently observed. There can be more than one modal value in the same variable

### **Measures of spread**
- Variance (variability from the mean):* The square of the standard deviation. It is also affected by outliers
- Standard deviation (concentrated around the mean): The standard amount of deviation (distance) from the mean. The std is affected by the outliers. It is the square root of the variance
- Percentiles: The value below which a percentage of data falls. The 0th percentile is the minimum value, the 100th is the maximum, the 50th is the median
- Minimum: The smallest or lowest value
- Maximum: The greatest or highest value
- The number of uniques (total distinct): The total amount of distinct observations
- Uniques (distinct): The distinct values or groups of values observed
- Skewness (symmetric): How much a distribution derives from the normal distribution
>> Explained Skew concept in the next section
- Kurtosis (volume of outliers): How long are the tails and how sharp is the peak of the distribution
>> Explained Kurtosis concept in the next section

### **Others**
- Count (size): The total sum of observations. Counting is also necessary for calculating the mean, median, and mode
- % highest unique (relativity): The proportion of the highest unique observation regarding all the unique values or group of values

## **Skewness**
In a perfect world, the data’s distribution assumes the form of a bell curve (Gaussian or normally distributed), but in the real world, data distributions usually are not symmetric (= skewed). Therefore, the skewness indicates how much our distribution derives from the normal distribution (with the skewness value of zero or very close).

There are three generic types of distributions:
- Symmetrical (median = mean): In a normal distribution, the mean (average) divides the data symmetrically at the median value or close.
- Positive skew (median < mean): The distribution is asymmetrical, the tail is skewed/longer towards the right-hand side of the curve. In this type, the majority of the observations are concentrated on the left tail, and the value of skewness is positive.
- Negative skew (median > mean): The distribution is asymmetrical and the tail is skewed/longer towards the left-hand side of the curve. In this type of distribution, the majority of the observations are concentrated on the right tail, and the value of skewness is negative.

Rule of thumbs:
- Symmetric distribution: values between -0.5 to 0.5.
- Moderate skew: values between -1 and -0.5 and 0.5 and 1.
- High skew: values <-1 or >1.
    
## **Kurtosis**
kurtosis is another useful tool when it comes to quantify the shape of a distribution. It measures both how long are the tails, but most important, and how sharp is the peak of the distributions. If the distribution has a sharper and taller peak and shorter tails, then it has a higher kurtosis while a low kurtosis can be observed when the peak of the distribution is flatter with thinner tails. There are three types of kurtosis:

- Leptokurtic: The distribution is tall and thin. The value of a leptokurtic must be > 3.
- Mesokurtic: This distribution looks the same or very similar to a normal distribution. The value of a “normal” mesokurtic is = 3.
- Platykurtic: The distributions have a flatter and wider peak and thinner tails, meaning that the data is moderately spread out. The value of a platykurtic must be < 3.

**The kurtosis values determine the volume of the outliers only.**
Kurtosis is calculated by raising the average of the standardized data to the fourth power. If we raise any standardized number (less than 1) to the 4th power, the result would be a very small number, somewhere close to zero. Such a small value would not contribute much to the kurtosis. The conclusion is that the values that would make a difference to the kurtosis would be the ones far away from the region of the peak, put it in other words, the outliers.
