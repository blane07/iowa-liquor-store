### Executive summary
##### A liquor store owner is looking to expand to a new location in Iowa
![Liquor Bottles](http://www.thecarycompany.com/media/img/page/glass-liquor-bottles.png "Liquor Bottles")
##### They have hired us to narrow their search from the entire state to just three counties
We used a dataset provided by Iowa of all Class E license liquor store transactions from January 2015 to March 2016. From this data we created a model and concluded that Johnson, Woodbury, and Scott are the best counties to establish a new liquor store in.

Nearly half of all class E license store transactions occurred in the top seven performing counties based on net profit. These counties were Polk, Linn, Scott, Johnson, Black Hawk, Potawattami, and Woodbury. We assumed that smaller counties have different economic forcing functions than larger counties, so we focused our analysis and the top seven counties.

We first compiled a list of top stores per county based on total net profit. Then we looked at profit per capita. The profit per capita is analogous to a “bang for buck” for the business owner. We then assess the marketplace saturation by creating a bar plot of people per store base on county. 

Next week created a linear regression for statistical inference between the different counties. The linear regression showed that locations, which are the counties, are statistically significant in explaining each transactions profit. This was an important find because it shows that the same transaction can occur in different counties, yet the profit will be different solely based on transaction’s location. The profit per transaction varies between $30.50 and $34. Saturated marketplaces, such as Black Hawk County, have lower profit per transactions.

The counties were ranked by profit per capita, marketplace saturation, and profit per transaction. These features were normalized so each feature carried equal weight and then multiply together for the final score. Please see the presentation for more details.

The model and approach has shortcomings. Trend information is valuable for business owners. When a business owner is sitting up a new store, they need to know about market trends. The data uses 15 months of transactions. This is insufficient to show market trends for the next 5, 10, or 30 years. This model assumes that each county’s performance will remain constant in the upcoming years. This is dangerous because what if a county had a above average year in 2015? Then the business owner would believe this county is better than it really is. Also, the model does not take into consideration businesses practices. Does the business value high-throughput? Or does it value a higher profit per transaction ratio? The model also weighs features equally. In actuality, the business would want to place more importance on some features than others. Other dimensions also exist, such as tax rates and other fees that vary from county to county.

*Please see the python code and presentation slides for more information*
