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

The dataset includes the following columns:

| Column Name         | Description                                |
|---------------------|--------------------------------------------|
| Campaign ID         | Unique campaign identifier                 |
| Company             | Organization running the campaign          |
| Campaign Type       | Type (Email, Influencer, Display, etc.)    |
| Target Audience     | Audience being targeted                    |
| Duration (days)     | Number of days campaign ran                |
| Channel Used        | Channel for campaign delivery              |
| Conversion Rate     | % of users converted after seeing the ad   |
| Acquisition Cost    | Cost to acquire each customer              |
| ROI                 | Return on investment                       |
| Date                | Campaign start date                        |
| Clicks              | Total clicks received                      |
| Impressions         | Number of times the ad was displayed       |
| Engagement Score    | User interaction score                     |
| Customer Segment    | Group classification of users              |

---

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