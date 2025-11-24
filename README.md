

# Taxi Trip Data Analysis Project

This project analyzes taxi trip data to uncover insights related to fare
amounts, trip distances, passenger counts, payment types, and overall
distribution patterns. Various visualizations and statistical tests are
included to support the findings.

## Contents

### 1. Distribution of Fare Amount

The histogram compares fare amounts for Card and Cash payments, showing
overall fare distribution and variation across payment methods.

### 2. Distribution of Trip Distance

This visualization shows the spread of trip distances for each payment
type, highlighting differences in travel patterns.

### 3. Normality Test (Q-Q Plot)

A Q-Q plot is used to visually assess the normality of the dataset.
Deviations from the reference line indicate skewness or heavy tails.

### 4. Passenger Count Distribution

A stacked horizontal bar chart displays the distribution of passenger
counts for Card and Cash transactions.

### 5. Payment Type Percentage

A pie chart illustrating the proportions of different payment types,
showing that Card payments dominate the dataset.

## Notebook

The full analysis, including data preprocessing, visualization, and
interpretation, is available in the Jupyter Notebook:\
`maximizing_revenue.ipynb`

## File References

The following plots are included in this project:

-   `hist_dist.png` --- Distribution of fare amount and trip distance\
-   `normality_test.png` --- Q-Q Plot for normality assessment\
-   `passenger_count_percentage.png` --- Passenger count distribution\
-   `payment_types_percentages.png` --- Percentage breakdown of payment
    types

## How to Use

1.  Open the notebook `maximizing_revenue.ipynb` to view the complete
    analysis.
2.  Review the images for quick insight into data patterns.
3.  Extend the project by adding:
    -   Predictive modeling
    -   Feature engineering
    -   Revenue optimization strategies

## Requirements

-   Python 3.x\
-   Jupyter Notebook\
-   Libraries:
    -   pandas
    -   numpy
    -   matplotlib
    -   seaborn
    -   scipy

## Purpose

The goal of this project is to analyze taxi trip data to identify
revenue-generating opportunities and understand customer behavior
through data visualization and statistics.




🟧 1. Distribution of Fare Amount (Card vs Cash)

https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20154210.png    

https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20154221.png
                           

✔ What this chart shows

This histogram compares fare amount distribution for Card and Cash payments.

✔ Key insights

Card payments dominate across almost all fare ranges, indicating that riders prefer digital payments.

Most fares cluster between $5 and $10, showing that the majority of trips are short to medium range.

Cash payments drop sharply after $10, while card payments remain more evenly spread—suggesting cash users usually take short rides.

Higher fares (e.g., $12–$18) are mostly paid by card, likely due to convenience and safety.

✔ What this means

Majority of the revenue comes from card users.

Cash users contribute fewer high-fare trips.

Fare distribution is right-skewed, meaning a small number of high-fare trips influence the upper range.

🟧 2. Distribution of Trip Distance (Card vs Cash)


https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20154928.png




✔ What this chart shows

This histogram compares trip distances for card and cash payments.

✔ Key insights

Most trips fall between 0.5 and 2.0 miles.

Shorter distances (0.5–1.0 miles) have high usage of both payment types, but card usage is still higher.

As distance increases (2–4 miles), card payments become significantly more common.

Very few long-distance trips are paid in cash.

✔ What this means

Card-paying customers tend to take longer trips.

Cash payments are concentrated in short, local rides.

Trip distance distribution is also right-skewed.

🟧 3. Q–Q Plot (Normality Check)


https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20155259.png




✔ What this chart shows

This Q–Q plot compares the sample quantiles of trip data with the theoretical quantiles of a normal distribution.

✔ Key insights

The points do not follow the diagonal line, especially in higher quantiles.

The upward curve indicates heavy right tail (positive skewness).

Data contains outliers and is not normally distributed.

✔ What this means

Statistical modeling techniques that assume normality may not be appropriate.

Log transformation or non-parametric models may be needed.

Real-world trip data usually follows skewed distributions, not normal ones.

🟧 4. Passenger Count Distribution (Card vs Cash)



https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20160059.png



✔ What this chart shows

A horizontal stacked bar chart comparing passenger count between cash and card payments.

✔ Key insights

Most rides have 1 passenger for both payment types.

Card payments dominate across all passenger categories.

Very few rides have 3, 4, or 5 passengers.

Cash payments decrease sharply when passenger count increases.

✔ What this means

Majority of trips are solo rides.

Higher passenger groups prefer card payments (likely because fares are shared or pre-planned).

Cash rides are simpler, quick, and mostly single-passenger.

🟧 5. Percentage of Payment Types (Overall Share)


https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20160222.png



https://github.com/subhaeng/-Hypothesis-testing-/blob/main/Screenshot%202025-11-24%20160238.png




✔ What this chart shows

A pie chart summarizing the overall share of payment types.

✔ Key insights

Card payments = ~74.9%

Cash payments = ~25.1%

✔ What this means

Digital payments dominate the dataset.

Riders strongly prefer card transactions for convenience, safety, and record-keeping.

Cash is still used, but mostly for short or small-value trips.

📌 Data Visualization Summary

The visual analysis reveals strong patterns in rider behavior and payment preferences:

Card payments dominate (≈75%), especially for long or high-fare trips.

Fare amounts and trip distances are both right-skewed, with most values clustered in a lower range.

Cash users primarily take short-distance and low-fare rides, showing different behavioral patterns.

Passenger count is mostly 1, and multi-passenger rides prefer card payment.

A Q–Q plot confirms the data is not normally distributed, showing skewness and outliers.

These insights help understand how customers interact with taxi services and guide further modeling, forecasting, or optimization.
