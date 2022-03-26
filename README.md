# 2012-CRT-TV-Retail-Audit-Market-Data-Analysis

Case study: The excel sheet represents retail audit market data for CRT Television in 2012, would you please prepare a presentation analysing the market in details?

first,
 The data is talking about CRT TV data in the 2012 retail audit market.

Tools used: python & power bi

Second, the implementation steps:

using Payton,
1) Understanding and describing the data: After importing and reading the data, the first impression of it is that it consists of several columns that include the name of the manufactured brand and its affiliated models, a description of the models, the expected financial returns from it, its price, and its digital and weighted distribution.
Looking inside the columns, we will find the first problem we meet, which is that the column of inches is a data type, although it is supposed to be digital, because TV sizes are measured in inches.
Then with the histogram, we will understand the distribution of the data more.

2) Preparing the data: we will check the missing values, and we will find that there are two columns in which there are two missing values. By looking at the data again, we find that the rows from which the values ​​are missing are the row of collecting numerical values ​​in the first, a description of other brands that are collected under the name of others, and the values ​​in it are all zero. There is no need for them in the analysis because they will not add anything new. Rather, in the operations on the columns, the total row can reveal other things, so they were deleted.

We will check duplicated, there is none.
With the describe function, we can notice that it contains outliers, but I think that they should not be modified in any way, because even if the value is little or far, it has no significance in the financial returns.

Then, moving forward with checking the columns, we will find a missing value in the inches column under the name unknown (hidden 😄), so we will adjust it in the mode of 21 and not mean or anything else because the sizes are fixed, so we cannot enter the float value in it.

We will find 13 missing values ​​in the DVD player column as N.A (hidden again 😄) We will adjust them to no DVD as the percentage of the DVD is completely wiped out by the most frequent value.

I like almost all the problems that I encountered in the data 😄

3) Analyzing the data to come up with useful products and information:
To begin with, we will divide the analysis into two parts, a section for the brand, and a section for studying the models of each brand, so that we can determine the profitable brands and, accordingly, their models that win and are well present in the market.
First the brands part: we will compare the percentage of sales values ​​of brands with the percentage of the numbers of their presence in the market so that we can determine the brands that are expected to return according to their numbers.
And we compare which size (inches) is expected to achieve profits in the market, as well as every type of screen, real flat or not, sound system, and finally the presence of DVD or not.

From here, we can determine the performance of brands in the market and their specifications.

Secondly, the model part: After determining the performance of the brands and knowing the most financial returns and the least of them, we need to determine the models with the most returns within these brands.

We worked a linear regression between the sales values ​​and numerical distribution once and widget distribution once, and we measured their p value and the two are highly significant in order to make sure of their impact on the output, why? So that we can market these products more according to their distribution and measure their performance and customer demand for them, and of course we will link them to the most profitable brands in the offer to determine the gains of each brand through its models and distribution.

Finally we got to the fun part, which is making a presentation of the data on power bi and the result is 😄
