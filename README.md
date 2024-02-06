# Linear Regression: Predicting Home Price

# Description: 
Using a dataset built from Zillow home listings, this project predicts home price based on various features from 600 homes listed on Zillow in Northwest Arkansas. The dataset consists of 300 sold homes and 300 homes still on market.

# Quick Conclusion: 
Number of Bathrooms: Positive impact, higher number leads to higher price.
Square Footage: Positive impact, larger size leads to higher price.
Number of Bedrooms: Negative impact (counterintuitive), might be due to smaller houses having more bedrooms or association with lower-priced areas.
Price Per Square Foot: Negative impact (counterintuitive), might be due to smaller houses having higher price per square foot.
Dollar Per Room: Positive impact, higher value leads to higher price.
City & Zip Code: Certain locations tend to have higher or lower average prices.
Model Performance:
All models show an average difference between predicted and actual prices.
Further Exploration:
Investigate the negative coefficients for Number of Bedrooms and Price Per Square Foot to understand the underlying reasons.
Consider alternative features or data transformations for improvement.

# Exploratory Analysis

Data is focused primarily on unsold homes in Rogers and Bentonville.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/a0f3d052-8e98-407c-84c4-bf87ec3b5183">

Data is focused primarily on sold homes in Rogers, Springdale and Bentonville.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/671a7eeb-1751-45de-982c-cdf5bd7a0db1">


There’s a positive correlation between price per square foot and total price of home.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/edaeef0b-240d-4d11-98de-f3ec3b152f2f">

The features with the highest correlation with price of home are: Dollar per room, price per square foot, number of bathrooms and square feet per room. So, size of home has a large impact on price of home.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/c0870523-3a07-4aa4-9db4-17509ded758f">


Highest priced homes are grouped together in the southeast corner while the majority of the houses are relatively priced similarly. 

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/f7f39b8f-e6e8-40c3-8b28-5d21f76df3a2">



The largest homes are grouped together in the southeast corner while the majority of the houses are similar sizes.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/7013ab24-42dd-4e18-b07a-6fb692d2f0a9">


Coeff


Number Of Bathrooms: 39750.645231<br>
Number of Bedrooms: -50203.671059 <br>
Price Per Square Foot: -341.936817 <br>
Square Feet: 352.630759 <br>
Year Built: 229.352336 <br>
Sold: 10066.328404 <br>
Square Feet Per Room: -1467.409630 <br>
Dollar Per Room: 3.920202 <br>
City_Cave Springs: 10882.239761 <br>
City_Centerton: -8181.273723 <br>
City_Fayetteville: 14571.799146 <br>
City_Little Flock: -63071.926165 <br>
City_Lowell: 25260.159886 <br>
City_Rogers: 56274.878207 <br>
City_Springdale: 48919.358633 <br>
Zip Code_72701: 26264.113787 <br>
Zip Code_72703: 35959.915619 <br>
Zip Code_72704: 22881.661546 <br>
Zip Code_72712: 63788.187282 <br>
Zip Code_72713: 19790.254844 <br>
Zip Code_72718: 10882.239761 <br>
Zip Code_72719: 52192.391545 <br>
Zip Code_72745: 25260.159886 <br>
Zip Code_72756: 19442.872042 <br>
Zip Code_72758: -26239.920000 <br>
Zip Code_72762: -19051.094573 <br>
Zip Code_72764: -2563.438600 <br>


# Description:
Number of Bathrooms: This feature has a positive impact on price, with each unit increase in Number of Bathrooms increasing the price by $39,750.65.

Number of Bedrooms: This feature has a negative impact on price, with each unit increase in Number of Bedrooms decreasing the price by -$50,203.67. This means that houses with more bedrooms tend to be more expensive, but the price increase is not as high as the price increase for houses with more bathrooms.

Price Per Square Foot: This feature has a negative impact on price, with each unit increase in Price Per Square Foot decreasing the price by -$341.94. This means that houses with higher price per square foot tend to be less expensive, which is counterintuitive. It might be because houses with higher price per square foot are smaller in size, and smaller houses tend to be cheaper.

Square Feet: This feature has a positive impact on price, with each unit increase in Square Feet increasing the price by $352.63. This means that larger houses tend to be more expensive.

Year Built: This feature has a positive impact on price, with each unit increase in Year Built increasing the price by $229.35. This means that newer houses tend to be more expensive.

Sold: This feature has a positive impact on price, with each unit increase in Sold increasing the price by $10,066.33. I am not sure what this feature represents, but it seems like it has a positive impact on price.

Square Feet Per Room: This feature has a positive impact on price, with each unit increase in Square Feet Per Room increasing the price by $1,467.41. This means that houses with more square footage per room tend to be more expensive.
Dollar Per Room: This feature has a positive impact on price, with each unit increase in Dollar Per Room increasing the price by $3.92. I am not sure what this feature represents, but it seems like it has a positive impact on price.

City: The city with the highest average price effect is City_Rogers, with an average price effect of $56,274.88. The city with the lowest average price effect is City_Little Flock, with an average price effect of -$63,071.93. This means that houses in City_Rogers tend to be more expensive than houses in City_Little Flock.

Zip Code: The zip code with the highest average price effect is Zip Code_72712, with an average price effect of $63,788.19. The zip code with the lowest average price effect is Zip Code_72758, with an average price effect of -$26,239.92. This means that houses in Zip Code_72712 tend to be more expensive than houses in Zip Code_72758.

# Results

# Unscaled Data:
<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/7e36bd78-c5f1-4372-b037-c299aa183f29">

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/5a58be54-ee47-4cab-bae4-75dc4663894a">

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/37edfa86-38f9-47bc-ba20-ccb3cc08001a">

Average Difference: $6654.58


# Min Max Scaler

Coeff

Number Of Bathrooms: 2.782545e+05 <br>
Number of Bedrooms: -3.012220e+05 <br>
Price Per Square Foot: -4.349436e+05 <br>
Square Feet: 3.316140e+06 <br>
Year Built: 3.187997e+04 <br>
Sold: 1.006633e+04 <br>
Square Feet Per Room: -3.197486e+06 <br>
Dollar Per Room: 4.981924e+06 <br>
City_Cave Springs: 1.088224e+04 <br>
City_Centerton: -8.181274e+03 <br>
City_Fayetteville: 1.457180e+04 <br>
City_Little Flock: -6.307193e+04 <br>
City_Lowell: 2.526016e+04 <br>
City_Rogers: 5.627488e+04 <br>
City_Springdale: 4.891936e+04 <br>
Zip Code_72701: 2.626411e+04 <br>
Zip Code_72703: 3.595992e+04 <br>
Zip Code_72704: 2.288166e+04 <br>
Zip Code_72712: 6.378819e+04 <br>
Zip Code_72713: 1.979025e+04 <br>
Zip Code_72718: 1.088224e+04 <br>
Zip Code_72719: 5.219239e+04 <br>
Zip Code_72745: 2.526016e+04 <br>
Zip Code_72756: 1.944287e+04 <br>
Zip Code_72758: -2.623992e+04 <br>
Zip Code_72762: -1.905109e+04 <br>
Zip Code_72764: -2.563439e+03 <br>

# Description:

Number of Bathrooms: This feature has a positive impact on price, with each unit increase in Number of Bathrooms increasing the price by $278,254.52.

Number of Bedrooms: This feature has a negative impact on price, with each unit increase in Number of Bedrooms decreasing the price by -$301,222.06.

Price Per Square Foot: This feature has a negative impact on price, with each unit increase in Price Per Square Foot decreasing the price by -$434,943.68. This means that houses with higher price per square foot tend to be less expensive, which is counterintuitive. It might be because houses with higher price per square foot are smaller in size, and smaller houses tend to be cheaper.

Square Feet: This feature has a positive impact on price, with each unit increase in Square Feet increasing the price by $3,316,140.66. This means that larger houses tend to be more expensive.

Year Built: This feature has a positive impact on price, with each unit increase in Year Built increasing the price by $31,879.97. This means that newer houses tend to be more expensive.

Sold: This feature has a positive impact on price, with each unit increase in Sold increasing the price by $100,663.28. I am not sure what this feature represents, but it seems like it has a positive impact on price.

Square Feet Per Room: This feature has a negative impact on price, with each unit increase in Square Feet Per Room decreasing the price by -$3,197,486.00. I am not sure what this feature represents, but it seems like it has a negative impact on price.

Dollar Per Room: This feature has a positive impact on price, with each unit increase in Dollar Per Room increasing the price by $4,981,924.40. I am not sure what this feature represents, but it seems like it has a positive impact on price.

City: The city with the highest average price effect is City_Rogers, with an average price effect of $56,274.88. The city with the lowest average price effect is City_Little Flock, with an average price effect of -$630,719.26. This means that houses in City_Rogers tend to be more expensive than houses in City_Little Flock.

Zip Code: The zip code with the highest average price effect is Zip Code_72712, with an average price effect of $637,881.87. The zip code with the lowest average price effect is Zip Code_72758, with an average price effect of -$262,399.20. This means that houses in Zip Code_72712 tend to be more expensive than houses in Zip Code_72758.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/bad932cb-0dc6-4b2d-8443-e9aeaba89a44">

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/9bb816df-f631-428a-853c-4713a5a5e8bb">

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/9e362afd-d513-4323-91fd-190364ffadf2">


Average Difference: $275835.22


# Standard Scaler

Coeff

Number Of Bathrooms: 43073.273361 <br>
Number of Bedrooms: -39582.754174 <br>
Price Per Square Foot: -45594.539067 <br>
Square Feet: 414275.316703 <br>
Year Built: 5051.451387 <br>
Sold: 5029.176056 <br>
Square Feet Per Room: -335553.302057 <br>
Dollar Per Room: 521793.846385 <br>
City_Cave Springs: 2421.387925 <br>
City_Centerton: -1736.085291 <br>
City_Fayetteville: 587.545413 <br>
City_Little Flock: -4680.250830 <br>
City_Lowell: 5984.964281 <br>
City_Rogers: 11877.148105 <br>
City_Springdale: 13464.085733 <br>
Zip Code_72701: 8690.178978 <br>
Zip Code_72703: 11773.380868 <br>
Zip Code_72704: 3070.164994 <br>
Zip Code_72712: 21752.075873 <br>
Zip Code_72713: 5650.893557 <br>
Zip Code_72718: 2421.387925 <br>
Zip Code_72719: 10794.014797 <br>
Zip Code_72745: 5984.964281 <br>
Zip Code_72756: 15064.542928 <br>
Zip Code_72758: 1943.348150 <br>
Zip Code_72762: -1831.335069 <br>
Zip Code_72764: 2687.795403 <br>

# Description:
Number of Bathrooms and Square Feet: Both features have positive coefficients, indicating that houses with more bathrooms and larger square footage tend to be more expensive.

Number of Bedrooms and Price Per Square Foot: These features have negative coefficients, suggesting that houses with more bedrooms and higher price per square foot tend to be less expensive. This might seem counterintuitive, but it could be due to factors like smaller houses having higher price per square foot, or more bedrooms being associated with lower-priced suburban areas.

Dollar Per Room: This feature has a positive coefficient, indicating that houses with higher dollar per room tend to be more expensive.

Specific Features:

Year Built: The positive coefficient suggests newer houses are generally more expensive.

Sold: The positive coefficient suggests that houses marked as "Sold" in your data might have sold for a premium compared to other factors. More context is needed to interpret this fully.

City: Several cities have positive coefficients, meaning houses in those locations tend to be more expensive than the baseline. Conversely, some cities have negative coefficients, suggesting they are generally less expensive.
Zip Code: Similar to cities, some zip codes have positive coefficients indicating higher prices, while others have negative coefficients suggesting lower prices.

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/446b9bc1-bdfa-4d24-a3bb-1e0222dddd4a">

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/1e3e9da5-9b57-43cd-8aaa-d427b2e3d653">

<img width="500" alt="image" src="https://github.com/Tannerbrodess/zillow_linear_regression/assets/159087577/efa974d7-8cad-4c71-bb9b-4f44e741eae2">

Average Difference: $35037.93


