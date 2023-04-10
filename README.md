### Will a Customer Accept the Coupon?

The notebook provides the following context of the problem to be solved:

> Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Data for 5 types of coupons were provided. These were for Coffee Houses, Affordable Restaurants (price < $20), More expensive Restaurants ($20-50), Bars, and Take Outs. 

Approximately 56.9% of all coupons are accepted by drivers. Here we analyze coupons for Bars and Coffee Houses in the Jupyter notebook [coupon_analysis.ipynb](https://github.com/sunukp/mlport/blob/main/coupon_analysis.ipynb).


## Summary of Findings

# Bar coupons
We followed the problem's prompt to investigate the coupon acceptance rate for various different groups that were offered Bar coupons.
The overall acceptance rate was 41.2%. By subsetting the dataset we found that those who visited bars more than 3 times per month had about 76.2% change of accepting the coupon. Acceptance rate of different groups are detailed in the accompanying notebook.

# Coffee House coupons
As the independent investigation, we chose to analyze the CoffeeHouse coupons. The goal here was to find specific user & contextual attributes that reach coupon acceptance rate of 80% or higher. We reached that goal by a mixture of the following attributes:
1. Visit frequency to CoffeeHouse more than once per month
2. Income less than $25,000
3. The driver doesn't have an urgent destination
4. The coupon destination can be reached within 15minutes.

## Next Steps and Recommendations

In the independent investigation, we came up with a concrete goal. However the method to reach that goal may be improved. A method to parallelize the search most likely exist. Such method should be preferred over ours, which was to narrow down the dataframe in sequence.
