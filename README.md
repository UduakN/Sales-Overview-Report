# Sales-Overview-Report

![image](https://github.com/UduakN/Sales-Overview-Report/assets/128192166/06106fed-251f-4b77-b9ba-6c85d939681e)

# Introduction

In modern commerce, data reigns supreme. The amalgamation of sales figures, consumer behaviour patterns, and geographic information presents a vase of insights that can redefine success for any business. This project dataset lies within this context. The project aims to extract invaluable insights that will drive innovative approaches and elevate the effectiveness of marketing, sales endeavours which include recognition. 

# About Dataset

The dataset consists of three tables, with each contributing unique dimensions to the overall narrative

1.	Orders table – Boasting 17 columns and 10,195 rows, this table serves as the backbone of our dataset.
   
2.	People table – It consists of 2 columns, 5 rows
   
3.	Return table – This table consist of 2 columns, 801 rows


# Tools Used

Microsoft Excel

Tableau

# Data Cleaning
Dataset was clean except for the data types which were changed where applicable.

# Tableau calculations

Total current year sales = IF YEAR([Order Date]) = {MAX(YEAR([Order Date]))} THEN [Sales] END

Total current year profit = IF YEAR([Order Date]) = {MAX(YEAR([Order Date]))} THEN [Profit] END

Total current year Qty = IF YEAR([Order Date]) = {MAX(YEAR([Order Date]))} THEN [Qty] END

Total previous year sales = IF YEAR([Order Date]) = {MAX(YEAR([Order Date]))}-1 THEN [Sales] END

Total previous year profit = IF YEAR([Order Date]) = {MAX(YEAR([Order Date]))}-1 THEN [Profit] END

Total previous year Qty = IF YEAR([Order Date]) = {MAX(YEAR([Order Date]))}-1 THEN [Qty] END

Minimum maximum sales = IF SUM([Total CY Sales])= WINDOW_MAX(SUM([Total CY Sales])) THEN SUM([Total CY Sales])
ELSEIF SUM([Total CY Sales]) = WINDOW_MIN(SUM([Total CY Sales])) THEN SUM([Total CY Sales])
ELSE NULL
END

Minimum maximum profit = IF SUM([Total CY Profit])= WINDOW_MAX(SUM([Total CY Profit])) THEN SUM([Total CY Profit])
ELSEIF SUM([Total CY Profit])= WINDOW_MIN(SUM([Total CY Profit])) THEN SUM([Total CY Profit])
ELSE NULL
END

Minimum maximum qty = IF SUM([Total CY Qty])= WINDOW_MAX(SUM([Total CY Qty])) THEN SUM([Total CY Qty])
ELSEIF SUM([Total CY Qty]) = WINDOW_MIN(SUM([Total CY Qty])) THEN SUM([Total CY Qty])
ELSE NULL
END




# Data Visualization

![image](https://github.com/UduakN/Sales-Overview-Report/assets/128192166/97a5349c-a3bf-4f81-bf92-cbfac618c0ea)


# Insights

1.	California's Dominance: Positioned at the forefront, California emerges as the powerhouse of mot sales with an impressive revenue of $457,658, accompanied by substantial profits amounting to $76,381. 

2.	Segment Insights: While the home office segment trails with a least share of 18.7% in sales, the consumer segment reigns supreme, commanding a commanding 50.56% share. The consumer segment is the primary driver of sales momentum.

3.	Top-performing Subcategories: With notable products like phones, chairs, storage solutions, tables, and binders shine brightly, collectively amassing substantial sales figures: phones lead the pack with an impressive $330,007, closely followed by chairs at $328,449, showcasing the diversified yet impactful array of sales-contributing products.

4.	Monthly Trends: November 2021 stands out as the best month in terms of sales, outperforming all previous months. In contrast to the equivalent months of the next year, March of the previous year, 2020, stands out as the peak of profitability. It is marked as the period of unmatched earnings.

5.	Yearly Profit Peaks: When compared to the same month in the following year, 2021, October 2020 stands out as the month with the most profitability, coming in at $16,243. This outlier highlights the one and only instance of extraordinarily profit.

6.	Sales Maestro - Anna Andreadi: Anna Andreadi stands out as a notable figure among the group of salespeople. With an excellent record, her sales abilities are evident, as seen by her astounding $725k in total sales. Her outstanding success establishes a new standard for great accomplishment and confirms her position as a trailblazer in the sales field

# Recommendations

1.	 Given California's prominence in sales and profitability, intensify efforts in marketing campaigns, localized initiatives, or strategic partnerships to further stronghold to amplify revenue streams.

2.	While the consumer segment thrives, explore avenues to enhance the engagement of the home office segment. Targeted promotions, exclusive offers, or personalized marketing strategies can invigorate this segment, tapping into untapped potential.

3.	Align marketing initiatives and promotional activities with temporal trends. Leverage the historical performance peaks in months like November for sales and March for profitability, crafting campaigns or promotions to capitalize on these high-performing periods.

4.	Investigate the outlier of October 2020 to discern the factors contributing to exceptional profitability. Understanding the dynamics behind this anomaly can unveil strategies or practices that could be replicated or adapted to boost profitability in subsequent years.

5.	Use Anna Andreadi's exceptional performance as a case study or inspiration for training and empowering other salespersons. Encourage knowledge sharing, mentorship programs, or incentivize best practices to elevate the overall sales team's performance.





