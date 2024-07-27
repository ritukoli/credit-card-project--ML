# credit-card-project--ML

1) started by performing an initial exploration to understand its structure, identify missing values, and gather basic statistics.
2) did not find any missing values in the data
3) droped the last 2 columns considering they werent required for further work that was to be done

   
4) Analyze the demographics of the credit card holders (e.g., age, salary, marital status) and visualize the distributions.
   # findings-of-the-analyses
   1) customer ranging from 40 to 60 are the maximum
   2) mostly people earn less that 40k
   3) number of married people is the highest

5) Explored how different demographics correlate with credit card limit, balance, and category. Identify any interesting patterns
   # findings-of-the-corelation
   1) # credilimit-by-customer-age
      1) The median credit limit (the line inside each box) varies by age but generally lies between 5000 and 15000.
      2)  Some age groups have more variation in their credit limits. For instance, younger customers (ages 26-36) and middle-aged customers (ages 37-50) show a higher number of outliers and a wider range of credit limits compared to older customers (ages 61-73).
      3)  The circles above the whiskers represent outliers, which are data points that lie outside 1.5 times the IQR above the upper quartile or below the lower quartile. There are many outliers, especially in younger age groups (e.g., 26-35), suggesting a few individuals in these groups have significantly higher credit limits.
      4)  The whiskers (lines extending from the boxes) show the range of the data excluding outliers. The range is generally wide, indicating high variability in credit limits across all age groups.

    2) # credilimit-by-income_category
       1) The median credit limit increases with income category:
Less than $40K: The median is around 5000.
$40K - $60K: The median is slightly higher than in the "Less than $40K" category.
$60K - $80K: The median is around 10000.
$80K - $120K: The median is around 15000.
$120K+: The median is the highest, around 25000.
Unknown: The median is around 10000.
        2)  There are many outliers in each category, especially in the lower income categories and the "Unknown" category. This suggests that while the majority of individuals have lower credit limits, there are a few individuals with significantly higher credit limits.
        3)  Higher income categories tend to have higher credit limits, as seen by the rising median and wider IQR in higher income categories.
      
      3) # Avg_Open_To_Buy-by-Marital_status
         1) The median Avg_Open_To_Buy (the line inside each box) is similar across different marital statuses, lying roughly between 5000 and 7000.
         2) There are numerous outliers in all categories, represented by circles above the whiskers. This suggests that, regardless of marital status, there are individuals with significantly higher Avg_Open_To_Buy values than the majority.
         3) There is no significant difference in the distribution of Avg_Open_To_Buy across the different marital status categories (Married, Single, Unknown, Divorced). All categories show similar medians, IQRs, and ranges.
      
7) used standardscaler and then trained model
