# Netflix-Engagement-Churn-Analysis using PowerBI
This project analyzes Netflix user engagement and churn behavior using Power BI. It explores churn rates, device usage, subscription impact, payment behavior, and promotional influence. Key insights include top-viewed devices, delayed payment effects, and retention trends. 📊🚀  🔹 Tools: Power BI, SQL, Python

The Netflix Engagement Churn Analysis project is designed to analyze customer engagement and churn behavior using a dataset (sourced from Kaggle). This Power BI dashboard provides a detailed breakdown of various metrics such as engagement rate, customer satisfaction, churn rate, payment history, and daily watch time across different devices.

Dashboard 1
![Screenshot 1](https://raw.githubusercontent.com/kaur-b76/Netflix-Engagement-Churn-Analysis/main/Screenshot%202025-03-12%20at%2023.28.23.png)


Dashboard 2
![Screenshot 2](https://raw.githubusercontent.com/kaur-b76/Netflix-Engagement-Churn-Analysis/main/Screenshot%202025-03-12%20at%2023.28.47.png)


I. Overall Metrics and Distributions:

- Customer Base: The dataset includes 3500 customer IDs, indicating a sizable user base.
- Engagement Rate: The average engagement rate is reported as 6.95 out of 10, suggesting a generally engaged user base.
- Customer Satisfaction: The average customer satisfaction score is 6.93 out of 10, indicating a moderately positive level of satisfaction.
- Churn Rate: The overall churn rate is approximately 11.34%. While this suggests that a majority of customers are retained, churn is still a factor.
- Payment History: A significant portion of customers have on-time payment history (approximately 77.97%), while a notable segment has delayed payments (approximately 22.03%).
- Promotional Offers: A large majority of customers did not utilize promotional offers.

II. Device Usage and Engagement:

- Daily Watch Time by Device: Daily watch time is distributed across various devices, with mobile and smart TVs being the most common platforms for viewing.
- Engagement Rate by Device Used: Mobile and Smart TV users exhibit higher engagement rates compared to other devices. This highlights the importance of these platforms for user engagement.

III. Factors Influencing Churn and User Behavior:

- Subscription Plans: Different subscription plans exhibit variations in subscription length and the number of profiles created. Premium plans tend to have longer average subscription lengths and a higher average number of profiles.
This suggests that premium plans may correlate with increased user investment in the platform.

- Age Segmentation: The age slicer in the dashboard indicates the ability to analyze churn and engagement across different age demographics. However, specific trends within age groups require further detailed analysis.

- Payment History: A notable portion of customers have delayed payments. This suggests that payment behavior may be a factor influencing churn. Further analysis is needed to quantify this relationship.

- Promotional Offers: Most customers have not used promotional offers. This suggests that promotional offer usage may not be a primary driver of overall engagement or churn within this dataset.

- Regional Analysis: The dashboard includes slicers for regions, enabling regional comparisons of income and churn. Based on the visualizations, average monthly income does not appear to significantly differ between churned and non-churned customers across most regions. This suggests that income, at a high level, may not be a primary driver of churn across regions in this dataset.

- Genre Preferences: The dashboard includes slicers for genres (Action, Comedy, Drama, Romance, Sci-Fi). This indicates the ability to analyze how genre preferences relate to user engagement and potentially churn.

IV. Interactive Analysis Capabilities:

The dashboards effectively utilize slicers for various dimensions, including age, payment history, subscription plans, regions, and genres. These slicers enable interactive exploration of the data, allowing users to analyze specific segments and filter data to identify trends.

The combined analysis provides a more comprehensive understanding of customer engagement and churn within the Netflix dataset.
Device usage patterns, subscription plan characteristics, and payment history are identified as potential factors influencing churn and user behavior.
Interactive slicers enhance the user's ability to explore the data, filter by specific dimensions, and uncover more granular insights.

V. Overview of the Dashboard Components
The dashboard consists of multiple visual elements, each contributing to the overall analysis of churn behavior:

- Key Performance Indicators (KPIs)
Engagement Rate: 6.95 – Represents the level of customer engagement with Netflix.
Total Customers Analyzed: 3,500 – The dataset includes 3,500 customer records.
Customer Satisfaction Score: 6.93 – The average satisfaction score among Netflix users.

- Age Distribution Filter
The age filter allows users to analyze churn and engagement trends across different age groups.
This provides insights into which age groups are more likely to churn and how engagement differs by age.

- Payment History (On-Time vs. Delayed)
77.97% (2.73K) of users pay on time, while 22.03% (0.77K) have delayed payments.
Delayed payments may correlate with a higher churn rate, as customers who struggle with timely payments may be less engaged.

- Churn Rate Analysis
11.34% of customers have churned (0.4K), while 88.66% remain active (3.1K).
Understanding what causes customers to churn is essential for improving engagement and retention strategies.

- Daily Watch Time by Device Used
Users watch Netflix on four primary devices:
Laptop: 3.08K hours (25.07%)
Mobile: 3.13K hours (25.49%)
Smart TV: 3.1K hours (25.23%)
Tablet: 2.97K hours (24.21%)
The usage is fairly evenly distributed, but trends in device preference may impact churn rates.

VI. How the Dashboard Works

- Interactivity
The Power BI dashboard allows interactive filtering, where users can select:
Age groups to see how churn varies by demographics.
Payment history categories to explore its effect on retention.
Device type filters to understand engagement behavior across different platforms.

- Data Relationships & Analysis
Engagement & Churn Relationship

A high engagement rate (6.95) suggests that most customers actively use Netflix.
Despite good engagement, 11.34% churned, which requires further investigation.
Impact of Payment History on Churn

Delayed payments are more common among churned users.
Customers who pay late might be more likely to cancel or abandon their subscriptions.
Device Usage Trends

Users watching on mobile and smart TVs have slightly higher watch times.
If a specific device group has a higher churn rate, Netflix can target engagement efforts accordingly.

VII. Findings & Conclusions

- Factors Influencing Churn
Low Customer Satisfaction (6.93)

Although engagement is decent, a satisfaction score of 6.93 is not high.
Netflix may need to improve content recommendations, streaming quality, or pricing strategies.
Delayed Payments & Churn

22% of users have delayed payments, and these customers may be more likely to churn.
Offering flexible payment options or reminders may reduce churn in this segment.
Age & Churn Trends

By filtering age groups, Netflix can identify whether younger or older customers churn more.
Targeted content or pricing adjustments could help retain specific age groups.
Device Preference & Engagement

Mobile & Smart TV users have the highest engagement.
If any device type correlates with higher churn, Netflix may need to optimize the viewing experience for that platform.

VIII. Recommendations to Reduce Churn

- Personalized Content Recommendations:Improve algorithm-driven recommendations to keep users engaged.
- Payment Flexibility: Introduce grace periods or loyalty discounts for late payers.
- Device Optimization: Ensure smooth streaming across all device types.
- Improve Customer Experience: Enhance UI/UX, customer support, and content library.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Furthermost, I have also done analysis in Jupyter Notebook using Python and below is the detailed explanation of the Exploratory Data Analysis (EDA) and model analysis.

The notebook contains 11 code cells related to Exploratory Data Analysis (EDA) and 7 code cells related to model analysis. 

# Exploratory Data Analysis (EDA)

Summary

The dataset is analyzed to understand user engagement patterns and churn behavior on Netflix. Here’s what was done:

**Dataset Overview:**

- Loaded the dataset and displayed the first and last few rows using df.head() and df.tail().
- Used df.info() to check data types and missing values.
- Used df.describe() to compute summary statistics.

**Handling Missing Data:**
- Checked for missing values using df.isnull().sum().
- Possible strategies like imputation or dropping rows were considered.

**Feature Exploration:**

- Analyzed the distribution of variables using histograms (df.hist()).
- Checked correlations between numerical features using df.corr().
- Boxplots and pairplots were used to identify outliers and relationships between variables.

**Churn Behavior Analysis:**

- Examined how engagement metrics (e.g., watch time, frequency of usage) relate to churn.
- Used value_counts() to analyze categorical variables like subscription types and user demographics.

**Model Analysis Summary**

The dataset was used to predict user churn with different machine learning models. Here’s what was done:

**Data Preparation:**

- The dataset was split into training and testing sets using train_test_split().
- Categorical variables were encoded if necessary.

**Model Selection:**

- Used models like Logistic Regression and Random Forest Classifier.
- Trained the models using fit() and made predictions using predict().

**Evaluation Metrics:**

- Measured accuracy using accuracy_score().
- Evaluated performance using confusion matrices (confusion_matrix()).
- Used ROC curves (roc_curve()) to compare model performance.

**Impact of Variables on Churn:**

Found key engagement factors affecting churn, such as:
- Watch time: Lower engagement correlates with higher churn.
- Subscription plan: Free-tier users are more likely to churn.
- Login frequency: Infrequent users have a higher churn probability.

## License & Usage Restrictions  
This repository is provided for viewing only. Downloading, modifying, or using this work for any purpose is strictly prohibited. See the [LICENSE](./LICENSE) file for details.




