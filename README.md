# Bank-Attrition-Analysis
**Overview Objective:**
Identify the key factors that influence customer attrition (“Exited”) in the bank and suggest strategies to reduce churn.

**Data Cleaning:** Standardized column names, converted blanks to NaN, imputed or dropped missing values, and engineered categorical bins for continuous variables.

**Data Analysis:** Conducted univariate, bivariate, and multivariate analyses to explore relationships between demographics, product usage, satisfaction, and churn.

**Data Visualization:** Employed histograms, box plots, bar charts, and heatmaps (using Matplotlib, Seaborn, and Plotly) to reveal patterns and correlations.

**Insights**: Discovered that low tenure, low satisfaction, inactive membership, and certain age/salary groups are strongly associated with higher churn rates.

**Deliverable:** A comprehensive Jupyter Notebook with annotated code, clean datasets, interactive visualizations, and a slide deck summarizing key findings and recommendations.

**Extended Overview**
**Data Collection & Cleaning**

**Source & Scope**: Loaded the Bank Customer Attrition dataset (≈ 10 k records, 20+ features) containing demographics, financials, product holding, and engagement indicators.
Preprocessing Steps:

Column normalization: Renamed to lowercase and replaced spaces/’-’ with underscores.

Null handling: Converted blank strings in gender, card_type, salary to NaN; imputed or dropped rows with critical missing entries in card_type, salary.

Feature engineering: Created categorical bins for tenure, age, credit score, balance, satisfaction score, salary, and number of complaints to facilitate grouped analyses.

**Data Analysis**
**Univariate Analysis**: Assessed distributions of all features; e.g., the majority of customers have a tenure of ≤ 5 years and credit scores between 600–800.
**Bivariate Analysis**: Explored churn rate vs. single variables—found that customers with tenure < 3 years and satisfaction score ≤ 3 have churn rates > 40%.

**Multivariate Analysis**: Investigated interactions (e.g., age & salary; credit score & number of products) revealing compounded risk factors, such as older customers with low balances and no active membership being most at-risk.

**Data Visualization**
**Techniques Used:**

Histograms & KDE plots to show distributions (age, salary).

Boxplots comparing balance and credit score by churn status.

Bar charts for categorical churn rates (gender, card type, product count).

Heatmaps of correlation matrix to highlight feature interdependencies.

Interactive dashboards (Plotly Express) for stakeholder exploration.

**Trend Analysis**
**
**Customer Lifecycle Patterns**: Identified a steep drop-off in retention after 2–3 years of tenure.

**Product Engagement:** Higher attrition among customers holding only one product; upsell opportunities (e.g., introducing additional products) could bolster retention.

**Satisfaction & Complaints: **Satisfaction scores ≤ 3 and any customer complaints increased churn likelihood by over 50%.

**Summary**
Through systematic EDA, the analysis pinpoints actionable levers—enhancing early tenure engagement, improving service satisfaction, targeting product cross-sells, and reactivating inactive members—that can reduce attrition.
