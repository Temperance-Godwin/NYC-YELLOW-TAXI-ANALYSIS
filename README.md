## INTRODUCTION
![Intro](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/intro.jpg)

Every day, thousands of yellow taxis crisscross the city, transporting locals, tourists, and business travelers. While the city pulses with this constant motion, questions emerge like when taxes are highest in demand and how long do trips last.

To make informed decisions about infrastructure, pricing models, traffic policies, and even driver support systems, we need to dig into the data.

As part of the strategic planning team for the New York City Transportation Authority, i stepped into the role of a data analyst tasked with uncovering insights from NYC Yellow Taxi trip data. By exploring patterns in trip duration, pickup and drop-off locations, fare structures, and time-based behaviors, this analysis supports data-driven decisions that can shape the future of urban mobility in New York City.

## PROBLEM STATEMENT
Increasing revenue is crucial for both long-term sustainability and driver satisfaction. This project seeks to leverage data-driven strategies to optimize earnings for taxi drivers. Specifically, investigations were made to check whether the method of payment influences the fare amount, focusing on the potential link between payment type and total fare.

## RESEARCH QUESTIONS
1. Is there a significant relationship between the total fare paid and the type of payment used?
2. Can customer behavior be influenced to prefer higher-revenue payment options without reducing customer satisfaction?
   
## OBJECTIVE
The primary aim of this project is to conduct an A/B test to assess whether there's a meaningful difference in fare amounts based on the customer's payment method. By using Python for statistical hypothesis testing and descriptive analytics, the aim is to uncover trends that can help drivers optimize their income. Specifically, the focus is on comparing credit card payments to cash payments to determine if one consistently results in higher fares.

## DATA SOURCE
Kaggle: Check data [here](https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data)

## DATA OVERVIEW
This analysis draws on a robust dataset from the New York City Taxi and Limousine Commission, containing detailed records of taxi trips. After applying data cleaning techniques and performing feature engineering, i isolated the essential variables needed for this investigation, including fare amount, payment type, trip duration, and passenger count.

## METHODOLOGY
**Descriptive Statistics:** Used to summarize and visualize key variables such as fare amount and payment method distribution.

**Hypothesis Testing:** A two-sample T-test was conducted to assess if there's a statistically significant difference in fare amounts between payment types.

**Regression Analysis:** Applied linear regression to examine the correlation between trip duration (derived from pickup and drop-off times) and fare amount.

View code [here](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/NYC%20Yellow%20Taxi%20Analysis.ipynb)

## KEY INSIGHTS

1. Trip and Fare Trends by Payment Type
Customers who paid using credit cards typically had longer trips and higher fares than those who paid in cash. This may suggest a tendency for riders to opt for card payments when taking longer or more expensive trips.

**Distribution of fare amount**
![Distribution](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/Distribution%20of%20fare%20amount.png)

**Distribution of trip distance**
![distance](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/Distribution%20of%20trip%20distance.png)


2. Customer Payment Preferences
Card payments made up 67.5% of all transactions, while cash accounted for just 32.5%. This points to a significant leaning toward card usage, possibly due to perceived ease, security, or available rewards.

![Preference](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/Total%20Percentage%20by%20Payment%20Type.png)

4. Passenger Count Trends
Single-passenger trips dominated card payment transactions, making up 40.08% of such payments. For cash payments, solo riders accounted for 20.04%. As the number of passengers increased, the proportion of both card and cash transactions dropped, suggesting that larger groups might prefer other transportation options or payment methods. These patterns underscore the importance of considering both the number of passengers and the payment method when analyzing taxi transaction data.

![Passenger count](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/Passenger%20count%20by%20Payment%20Type.png)

## HYPOTHESIS TESTING

**Null Hypothesis (H₀):** There is no difference in average fare between card-paying and cash-paying customers.

**Alternative Hypothesis (H₁):** There is a significant difference in average fare between card and cash transactions.

**Q-Q plot of Fare Amount**

![QQ](https://github.com/Temperance-Godwin/NYC-YELLOW-TAXI-ANALYSIS/blob/main/Q-Q%20plot%20of%20fare%20amount.png)

*Using a T-statistic of 169.21 and a p-value below 0.05, we reject the null hypothesis. This outcome indicates a statistically significant difference in fare amounts between the two payment methods.*

## RECOMMENDATIONS
1. Promote the use of credit cards to help drivers earn more per trip by:
- Displaying in-app prompts or messages during the booking process that highlight the benefits of using card payments, such as faster checkouts or contactless convenience.
- Equiping drivers with small signs or digital displays inside the vehicle encouraging card payments.
- Providing training for drivers to politely suggest card payment when appropriate.

2. Introduce incentives, such as discounts or loyalty programs, to encourage customers to choose card payments by:
- Collaborating with payment providers to offer limited-time promotions, such as small discounts (e.g., $1 off) for customers who pay with a card.
- Launching loyalty rewards programs where customers earn points for each card transaction, redeemable for future discounts or free rides.
- Offering bundled deals—such as a discount on a return trip—exclusively for card users.

3. Ensure the payment system is smooth, secure, and reliable to increase customer confidence and preference for card transactions by:
- Upgrading in-vehicle payment terminals to ensure quick and reliable card processing, including contactless and mobile payment options (Apple Pay, Google Pay, etc.).
- Improving the in-app experience by allowing customers to securely save their card details for one-click payments.
- Ensuring transparent digital receipts are automatically sent post-ride to build trust and reduce disputes.

4. Leverage Data for targeted communication by:
- Analyzing customer payment behavior and send personalized messages or push notifications to frequent cash users, highlighting the advantages of card payments.


5. Monitor and Measure Impact Continuously by:
- Tracking changes in payment method trends over time after implementing incentives or interface changes.
- Collecting feedback from both drivers and riders to refine the strategies.
- Using periodic A/B tests to validate whether new tactics effectively increase card usage without compromising customer experience.

![Thank you](https://github.com/Temperance-Godwin/Forbes-world-billionaires-2022/assets/156975460/f6563ba6-1ad6-4d34-a3f3-8e7fbdf654df)

## Thank you for following through.


