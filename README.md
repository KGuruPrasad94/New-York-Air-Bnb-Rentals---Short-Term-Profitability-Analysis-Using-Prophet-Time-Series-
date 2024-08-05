# Project Summary: New York Airbnb Rentals – Short Term Profitability Analysis

Objective:
To identify the best zip codes in New York City for investing in 2-bedroom properties for short-term rentals, based on profitability. The goal is to develop a scalable data product to assist in investment decisions.

Data Sources:

	1.	Airbnb Data: CSV files containing various attributes of Airbnb listings in NYC.
	2.	Zillow Data: Zip code level data containing median house prices from 1996 to 2017.

Approach:

	1.	Data Wrangling and EDA:
	•	Airbnb Data: Cleaned and standardized the data by handling null values, correcting erroneous entries, and transforming the format for consistency.
	•	Zillow Data: Focused on renaming columns, handling time-series data, and addressing skewness in house prices.
	•	Joining Data: Combined Airbnb and Zillow datasets using zip codes and included forecasted future house prices for comprehensive analysis.
	2.	Feature Engineering:
	•	Selected key features such as neighborhood, room type, property type, number of bedrooms, availability, and price.
	•	Created new variables like annual revenue and forecasted house prices for 5, 10, and 15-year periods.
	3.	Time Series Forecasting:
	•	Used the Prophet algorithm to forecast future house prices based on historical data.
	•	Chose the 5-year forecast period for ROI calculations due to its balance between short-term and long-term predictability.
	4.	Profitability Analysis:
	•	Break-even Analysis: Calculated the payback period to determine the time required to break even on the initial investment.
	•	ROI Calculation: Evaluated the profitability over a 5-year period by combining rental income and forecasted property appreciation.

Assumptions:

	•	75% occupancy rate for Airbnb rentals.
	•	Cash purchases without mortgage considerations.
	•	Homogeneous property characteristics within each locale.
	•	Final prices in Airbnb data are assumed without discounts or additional fees.
	•	Investment start date set to June 2017.
	•	Only zip codes with more than 15 listings were considered for analysis.

Findings:

	1.	Break-even Analysis:
	•	Average payback period for NYC listings is 28 years.
	•	Zip codes 10036, 10022 (Manhattan), 11231 (Brooklyn), 10025 (Manhattan), 11215, and 11217 (Brooklyn) have quicker break-even times.
	•	High-demand zip codes with numerous listings tend to achieve break-even points faster.
	2.	ROI Analysis:
	•	Average ROI for NYC listings over 5 years is 28.61%.
	•	Zip codes 10028 (Manhattan), 11231 (Brooklyn), 10128, 10021, 10011, 10023, and 10014 (Manhattan) produce higher returns than the average.
	•	Zip codes with higher listings tend to have lower ROI, suggesting a need to identify the best-performing neighborhoods within these zip codes.

Conclusion:

	•	Best Zip Codes for Investment: Based on the payback period, 10036, 10022 (Manhattan), and 11231 (Brooklyn) are the best zip codes for quick returns. For ROI, 10028 (Manhattan), 11231 (Brooklyn), and 10128 (Manhattan) are top performers.
	•	Investment Strategy: Focus on high-demand areas with moderate listings to optimize both break-even time and ROI.

Future Steps:

	•	Perform sentiment analysis on text columns to better understand successful Airbnb listing attributes.
	•	Obtain square footage data to enhance price analysis across different neighborhoods.
	•	Incorporate additional expenses and pricing variations for a more comprehensive analysis.
	•	Secure more zip code data to explore untapped locations in NYC.
	•	Explore alternative time-series models like ARIMA for better seasonality trend analysis.

This project highlights the importance of thorough data cleaning, feature engineering, and robust modeling techniques in making informed real estate investment decisions.
