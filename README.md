# Bank-Churn
**Bank Churn Analysis Dashboard 💰**

An interactive Power BI dashboard that explores customer churn behavior, uncovering key patterns through dynamic visuals and KPIs.

**📌 Project Description**

This project analyzes customer churn in a retail bank to identify customer churn patterns, financial impact of churn, and understand high-value customer behaviour. It is designed leveraging Power BI, Power Query and SQL to provide executive-level KPIs, detailed churn insights, and a dedicated high-value customer analysis. The dashboard includes drillthrough analysis, interactive slicers, and dynamic field parameters to enhance decision-making.

**🔍 Problem Statement**

Customer churn is one of the biggest challenges for banks, leading to revenue loss and reduced market share.
The goal of this project is to:
- Identify key churn drivers and patterns, including high-value customer churn and related balance loss
- Quantify the financial impact of churn
- Highlight areas of improvement to reduce churn
- Design targeted retention strategies for high-churn segments and estimate the potential balance saved
- Provide executives with actionable insights for decision-making

**📋 Methodology**

_**Data Preparation:**_

- Imported raw CSV into SQL & Power Query for cleaning
-	Performed transformations: removing duplicates, fixing datatypes, standardizing text (Trim, Clean, Replace, Capitalize Each Word)
-	Created custom columns for segmentation: Credit Score Bins, Age Brackets, Income Categories, Customer Value Segments

_**Data Modeling & DAX:**_

-	Built measures: Total Customers, Active Customers, Churned Customers, Retention Rate, Churn Rate, Balance Lost by Churn, etc.
-	Created a field parameter to dynamically switch visuals (Income vs Customer Value)

_**Visualization (Power BI):**_
-	Dashboard structured into 3 sections + drillthrough with slicers, KPIs, and navigation buttons
-	Bookmarks for reset-to-default page removing all applied filters


**🛠️ Tools Used**

SQL, Power Query, Power BI (DAX, Visualizations)

**📊 Data Source**

This dataset has been sourced from Maven Analytics Data Playground. 

https://mavenanalytics.io/data-playground

**💡 Key Insights**

**_Overall Performance_**
- The bank’s overall churn rate is 20.37%, leading to a total balance loss of $185.6M.
- Inactive customers churn at nearly double the rate of active customers (26.85% vs 14.27%).
- If the current churn trend continues, the annual financial risk is ~$155.8M in lost balances.
  
**_Key Churn Drivers_**
- Tenure: Customers with 0 years of tenure churn at 23%, indicating onboarding/early engagement is a major pain point.
- Credit Score: Low-credit customers (300–579) churn at 22.02%, above average; mid-score segment (580–669) holds the largest base of 3,331 customers.
- 	Geography: Churn is highest in Germany (32.44%), causing $97.97M in balance loss. France has the largest customer base, but Spain shows higher churn           proportions in High-Value segments.
- Age Bracket: Churn peaks in the 46–55 age group (50.57%) despite being a mid-sized segment. The 18–25 group churns the least (7.53%).
- Products: Customers with 4 products have 100% churn, while those with 2 products are most stable (7.58%).

**_High-Value Customers (HVs)_**
- HVs make up 24.8% of the base but account for 60.14% of average balance lost.
- Their churn rate (22.90%) is higher than regular customers (19.53%).
- Total balance lost from HV churn = $68.68M.
- Churn is heavily concentrated in the 56–65 age group (60.31%).
- By geography, HV churn is highest in Germany (29.74%), moderate in Spain (21.47%), and lowest in France (16.88%).
- HV tenure churn is volatile, peaking at 10 years (26.61%).
  
**_Other Observations_**
-	Income category is not a strong churn differentiator, but high-income customers represent the largest base (5,010) and contribute more to churn in absolute numbers.
-	Credit card ownership and gender show no significant correlation with churn.

**📈 Real-World Impact & Applications**

-	**Customer Retention Strategies**: Helps prioritize retention efforts on high-value customers with higher churn risk.
-	**Revenue Protection**: Quantifies financial impact of churn, enabling management to estimate cost of inaction.
-	**Segmentation-based Interventions**: Identifies vulnerable age brackets, income categories, and product holders for targeted campaigns.
-	**Executive Decision-Making**: High-level KPIs for quick monitoring, with drillthrough capability for deeper insights.
-	**Scalable Approach**: The framework can be applied to other financial institutions to monitor churn and improve retention strategies.

**📄 Dashboard Pages**

_**Executive Overview**_

![Executive Overview](https://github.com/abhilashini811/Bank-Churn-Analysis/blob/main/Executive_Overview.PNG)

_**Churn Overview**_

![Churn Overview](https://github.com/abhilashini811/Bank-Churn-Analysis/blob/main/Churn_Overview.PNG)

_**High Value Customers**_

![High Value Customers](https://github.com/abhilashini811/Bank-Churn-Analysis/blob/main/High_Value_Customers.PNG)

_**Churn Balance (Drillthrough Page)**_

![Churn Balance](https://github.com/abhilashini811/Bank-Churn-Analysis/blob/main/Churn_Balance-Drillthrough_Page.PNG)



