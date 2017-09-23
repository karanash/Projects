We have found some issues in data which we cleaned - 

FILE IMPORT NODE-
We found some variables as redundant because they could be calculated from other variables.
So, we rejected those variables -
1. Average Sales per customer
2. Average sales per item
3. All distances measured in feet


REPLACEMENT NODE -
1. Sunny and sunny were mentioned separately. Replaced sunny with Sunny.
2. Same was the case with cloudy and Cloudy. Replaced cloudy with Cloudy.
3. Discount was having negative values. We assumed that negative discount values do not make sense, so converted negative values to zero.

IMPUTE NODE -
1. We have imputed 'Number of Japanese tourists entered' as it was having missing values.
This factor may be dependent on Outlook, Temperture, Holiday etc. So, we used Tree method to impute missing values.

TRANFORM VARIABLES -
1. We found Total Sales as rightly skewed. So we used Square root to transform it.
2. We found Yen-Won Ratio as left skewed. So, we used Formula = (Yen-Won Ratio)^4
3. Also, there were some decimal places attached with imputed Number of Japanese tourists. So, used Floor function to remove that.

