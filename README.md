## 📄 Project Summary

This project presents a full-scale analysis of marketing campaign data to uncover insights into performance across channels, customer segments, and time. The dataset includes metrics such as clicks, impressions, ROI, CPC, and conversion rates from multiple companies and campaign types.

The analysis was conducted as the final project of a 60-day, 6-project data analytics challenge and demonstrates practical skills in data wrangling, exploratory data analysis, KPI engineering, and interactive dashboard creation using Power BI.

---

### ✅ Objectives

- Identify the most cost-effective and high-performing marketing channels
- Understand customer segment behavior and conversion patterns
- Track seasonal and temporal trends in campaign success
- Provide actionable insights through dynamic data visualization

---

## 🛠 Tools & Technologies Used

| Tool       | Purpose                                         |
|------------|-------------------------------------------------|
| Python     | Data wrangling, EDA, feature engineering        |
| Pandas     | Data cleaning and manipulation                  |
| Seaborn    | Visual exploration and correlation plots        |
| Power BI   | Dashboard creation and KPI visuals              |
| DAX        | Custom metrics in Power BI                      |
| GitHub     | Documentation and version control               |


---

## 📊 Dataset Overview

The dataset includes campaign-level records with the following attributes:

| Column              | Description                                  |
|---------------------|----------------------------------------------|
| Campaign ID         | Unique identifier for each campaign          |
| Company             | Campaign-owning company                      |
| Campaign Type       | Type of campaign (Email, Influencer, etc.)   |
| Channel Used        | Platform used for delivery                   |
| Customer Segment    | Targeted audience segment                    |
| Duration            | Number of days campaign lasted               |
| Clicks              | Total user clicks                            |
| Impressions         | Total ad views                               |
| Acquisition Cost    | Cost to acquire customers                    |
| Conversion Rate     | Proportion of conversions                    |
| ROI                 | Return on investment                         |
| Engagement Score    | Internal metric for interaction              |
| Date                | Campaign launch date                         |

---

## 🔧 Data Cleaning Summary

- Converted `Date` column to datetime format  
- Ensured numeric types for all quantitative columns  
- Filled missing `Engagement Score` with column mean  
- Labeled missing `Customer Segment` as `"Unknown"`  
- Removed duplicates and verified unique `Campaign ID`s  
- Created new features such as `CTR` and `CPC`

---

## 📈 EDA Highlights

### ✅ Univariate Analysis
- Most campaigns ran between **7–15 days**
- Impressions and Clicks were **right-skewed**
- Email and Social Media were the most used campaign types

### ✅ Bivariate Analysis
- **Clicks vs Impressions**: Strong positive correlation
- **CPC vs ROI**: Inverse relationship (higher CPC → lower ROI)
- **Engagement vs Conversion Rate**: Positive correlation

---

## 🔍 Correlation Analysis

```python
import seaborn as sns
import matplotlib.pyplot as plt

corr = df[['Clicks', 'Impressions', 'CPC', 'ROI', 'Conversion rate', 'Engagement score']].corr()
sns.heatmap(corr, annot=True, cmap='coolwarm')
plt.title('Correlation Heatmap')
plt.show()

## 📈 Power BI Dashboard Structure

### Page 1: Executive Overview
- KPIs: Total Campaigns, ROI, CPC, CTR, Conversions
- ROI & Conversion Trends
- ROI by Campaign Type and Company
- CPC vs ROI Scatter Plot
- Top Campaigns by ROI

### Page 2: Channel & Audience Summary
- ROI by Channel
- Engagement Score per Channel
- Conversion Rate by Customer Segment
- CPC by Channel
- Campaign Count by Channel
- ROI & CTR Summary Table

### Page 3: Time & Segment Trends
- Monthly ROI and Engagement Trends
- Campaign Volume over Time
- Conversion Rate Trends
- ROI by Customer Segment
- Monthly KPI Comparison Table

---

## 📌 Key Insights

- **Email and Facebook** campaigns delivered the highest ROI.
- **Outdoor Adventurers** and **Foodies** were top converting segments (~8%).
- **CPC** stayed consistently around $22.75 across all channels.
- **Q1 campaigns** outperformed all other timeframes in ROI and Engagement.
- High clicks didn’t always lead to conversions, indicating drop-off post-click.

---

## ✅ Recommendations

- Scale high-ROI campaigns on Email, Facebook, and Google Ads.
- Prioritize content for segments like Foodies and Outdoor Adventurers.
- Improve landing pages and funnel experience to reduce drop-offs.
- Schedule major campaigns in Q1 when audience engagement peaks.
- Use stable CPC values to focus on creative and targeting effectiveness.

---

## 🧾 Conclusion

This marketing campaign analysis project provided valuable insights into how various campaigns performed across channels, customer segments, and timeframes. 

Using a combination of **Python**, **Power BI**, and **DAX**, we were able to:

- Clean and transform raw marketing data into actionable metrics
- Analyze click-through, conversion, and cost-efficiency trends
- Build an interactive, dynamic dashboard tailored for business decision-makers
- Deliver a structured final report that highlights performance gaps and growth opportunities

The project clearly demonstrates that **timing**, **targeting**, and **channel selection** play more critical roles than raw budget spend alone. Email and Facebook proved to be the most reliable performers, while certain segments (like Outdoor Adventurers and Foodies) responded best to targeted marketing efforts.

This work serves not only as a portfolio piece but also as a decision support tool for marketing teams aiming to improve ROI and engagement across campaigns.

---

## 🔮 Future Work

To further enhance this analysis and scale it for enterprise use, the following improvements are proposed:

- 🔄 **Real-Time Data Integration**: Connect Power BI to a live marketing database with scheduled refreshes
- 🤖 **Predictive Modeling**: Use machine learning to forecast ROI and conversion rates based on campaign attributes
- 🧪 **A/B Testing Simulation**: Evaluate campaign variants by simulating audience responses across segments
- 📅 **Campaign Scheduler Tool**: Recommend best launch windows based on historical trends
- 🧠 **Text & Sentiment Analysis**: Analyze campaign copy and content performance using NLP techniques
- 📈 **Multi-touch Attribution**: Explore deeper customer journeys across multiple channels

These additions would expand the current dashboard from a performance analyzer to a **proactive strategy platform** for marketing optimization.
