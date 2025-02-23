# Coupon Acceptance Analysis

## Project Overview

This project analyzes a dataset of coupon offers and customer acceptance to identify factors influencing coupon redemption. The goal is to provide insights that can help businesses optimize their coupon strategies. We focused on analyzing the "Bar" and "CoffeeHouse" coupon groups to understand the characteristics of customers who are more likely to accept these coupons.

## Dataset

The dataset used in this analysis is `coupons.csv`, available in data/coupons.csv). It contains information about coupon offers, customer demographics, and acceptance outcomes.

## Project Structure

* `coupons_analysis.ipynb`: Jupyter Notebook containing the analysis code.
* `README.md`: This file, providing an overview of the project.

## Data Cleaning and Preprocessing

* **Missing Values:**
    * The 'car' column, which had approximately 99% missing values, was removed.
    * Missing values in 'Bar', 'CoffeeHouse', 'CarryAway', 'RestaurantLessThan20', and 'Restaurant20To50' were imputed using the mode (most frequent category).
* **Data Types:**
    * Relevant columns were converted to categorical data types for appropriate analysis.

## Analysis

### Bar Coupons Analysis

#### Problem Statement

The problem addressed was to identify the characteristics of customers who accept bar coupons.

#### Findings

* **Acceptance Rate:** Approximately 41% of bar coupons were accepted.
* **Bar Visit Frequency:** Customers who visit bars more than once a month were more likely to accept bar coupons.
* **Demographics:**
    * Customers without children present were more likely to accept bar coupons.
    * Customers not widowed were more likely to accept bar coupons.
    * Customers under the age of 30 were more likely to accept bar coupons.
    * Customers who visit cheap resturants more than 4 times a month and have an income less than 50k were more likely to accept bar coupons.
* **Complex Conditions:** Customers who meet any of the following conditions were more likely to accept bar coupons:
    * Bar visits > 1/month, not a kid, not widowed.
    * Bar visits > 1/month, under 30.
    * Cheap restaurant visits > 4/month, income < 50K.

#### Visualizations

* Countplots and stacked bar plots were used to visualize the relationships between customer demographics, bar visit frequency, and coupon acceptance.

#### Actionable Items

* Target bar coupons towards frequent bar-goers, individuals without children, younger individuals, and those who are price-sensitive.
* Consider partnerships with cheap restaurants to distribute bar coupons to customers with lower incomes.

#### Next Steps and Recommendations

* Perform statistical tests to confirm the significance of observed differences.
* Explore other variables and their impact on bar coupon acceptance.
* Consider time of day, weather, and location as potential factors.
* Further refine the targeted marketing strategy based on the identified customer profiles.

### CoffeeHouse Coupons Analysis

#### Problem Statement

The problem addressed was to identify the characteristics of customers who accept coffeehouse coupons.

#### Findings

* **Acceptance Rate:** The overall acceptance rate for CoffeeHouse coupons was calculated.
* **Passenger:** People traveling alone or with a partner were more likely to accept CoffeeHouse coupons.
* **Time of Day:** Afternoon and evening hours showed a higher acceptance rate.
* **Weather:** Sunny weather correlated with higher acceptance rates.
* **Occupation:** Students and those in management occupations showed a higher acceptance rate.
* **Temperature:** Higher temperatures seemed to correlate with slightly higher acceptance.
* **Income:** Medium-income people were more likely to accept CoffeeHouse coupons.

#### Visualizations

* Countplots and box plots were used to visualize the relationships between customer demographics, time of day, weather, temperature, and coupon acceptance.

#### Actionable Items

* Target CoffeeHouse coupons towards individuals traveling alone or with a partner, during afternoon and evening hours, when it is sunny, and towards students and those in management occupations.
* Consider offering CoffeeHouse coupons to medium-income customers.

#### Next Steps and Recommendations

* Perform statistical tests to confirm the significance of observed differences.
* Explore interactions between variables (e.g., time of day and passenger).
* Investigate other coupon groups using this approach.
* Refine the targeted marketing strategy based on the identified customer profiles.

## Conclusion

This analysis provides valuable insights into the factors influencing bar and coffeehouse coupon acceptance. By understanding the characteristics of customers who are more likely to accept these coupons, businesses can optimize their coupon strategies and improve their marketing effectiveness.
