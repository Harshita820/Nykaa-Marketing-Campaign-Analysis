# Nykaa Marketing Campaign Performance & Funnel Analysis

## Project Overview
This project analyzes Nykaa marketing campaign data to understand campaign effectiveness, customer conversion, and marketing spend efficiency.

**Core business question:** How can Nykaa improve conversions and revenue while using its marketing budget more efficiently?

## Business Objectives
- Compare campaign types by ROI, revenue, spend, and conversion rate.
- Identify drop-offs in the conversion funnel.
- Explore relationships between CTR, engagement, and conversion.
- Identify promising customer segments, channels, and campaign characteristics.
- Find high-ROI campaigns with relatively low spend and high-revenue campaigns with poor ROI.
- Turn findings into actionable marketing recommendations.

## Business Questions
1. Which campaign types generate the highest ROI?
2. Which campaign types generate the most revenue and conversions?
3. Are campaigns generating revenue efficiently, or simply spending more?
4. Where is the largest drop-off in the funnel?
5. Is CTR associated with conversion rate?
6. Which customer segments perform best?
7. How are engagement and conversion related?
8. How does campaign language relate to performance?
9. Which channels are associated with stronger results?
10. Do campaigns using more channels perform differently?
11. Which campaigns achieve high ROI with relatively low spend?
12. Which campaigns generate high revenue but poor ROI?

## Dataset
The dataset includes campaign-level fields such as `Campaign_ID`, `Campaign_Type`, `Target_Audience`, `Duration`, `Channel_Used`, `Impressions`, `Clicks`, `Leads`, `Conversions`, `Revenue`, `Acquisition_Cost`, `ROI`, `Language`, `Engagement_Score`, `Customer_Segment`, and `Date`.

## Key Metrics
Using the dataset's stated spend definition:

```text
Spend = Acquisition_Cost × Conversions
ROI = (Revenue - Spend) / Spend
CTR = Clicks / Impressions × 100
Conversion Rate = Conversions / Clicks × 100
Lead Rate = Leads / Clicks × 100
Lead-to-Conversion Rate = Conversions / Leads × 100
```

**Conversion funnel:** `Impressions → Clicks → Leads → Conversions`

## Analysis and Key Findings

### Campaign Performance
- Social Media and Paid Ads showed the highest ROI in the analysis.
- Influencer and Social Media campaigns showed the highest conversion rates.
- Influencer, Social Media, and Paid Ads generated the highest revenue.
- Paid Ads and Influencer campaigns also had relatively high spend.
- Email showed weaker returns at the campaign-type level.

**Implication:** Compare profitability alongside revenue and spend; high revenue alone does not necessarily mean high ROI.

### Top- and Bottom-Performing Campaigns
The top 10 ROI campaigns were mainly Paid Ads and Influencer campaigns and were associated with engagement scores around 24–30 and conversion rates around 5.5%.

The bottom 10 campaigns had negative ROI, engagement scores around 2–6, and conversion rates around 0.2%.

**Implication:** Use strong campaigns as benchmarks and investigate weaker campaigns before pausing or redesigning them.

### Conversion Funnel
Around 8.5% of impressions became clicks, more than 40% of clicks became leads, and more than 55% of leads became conversions.

**Implication:** The largest opportunity appears to be improving the impressions-to-click stage through more relevant creative, messaging, targeting, offers, and calls-to-action.

### CTR vs Conversion Rate
The correlation between CTR and Conversion Rate was **0.714**, indicating a strong positive association in this dataset.

**Implication:** Campaigns with higher CTR tended to have higher conversion rates. Correlation does not prove causation.

### Engagement vs Conversion
The chart showed a positive relationship between Engagement Score and Conversion Rate.

**Implication:** Encourage meaningful engagement, but evaluate it alongside conversions, ROI, and revenue.

### Customer Segmentation
Working Women and Premium Shoppers showed strong overall performance in the analysis, while Youth showed weaker performance on several measures.

**Implication:** Prioritize promising segments for further testing and investigate weaker performance before making broad budget changes.

### Language Analysis
Hindi campaigns showed strong results across reported measures, while English campaigns showed weaker engagement, conversion, and revenue results in this analysis.

**Implication:** Use stronger-performing language campaigns as a benchmark and investigate differences in audience, creative, and targeting.

### Channel and Multi-Channel Analysis
Instagram showed strong associated performance in the reported channel analysis. Campaigns using more channels were also associated with higher ROI and revenue.

**Implication:** Treat these as signals for further testing, not proof that a single channel caused the outcome. Multi-channel campaigns make individual-channel attribution difficult.

### Spend Efficiency
Higher spend did not consistently correspond to higher revenue or ROI. Some relatively low-spend campaigns achieved high ROI.

**Implication:** Prioritize efficient returns rather than automatically increasing budgets. Review high-spend, low-ROI campaigns and validate findings before reallocating substantial budget.

## Recommendations
1. **Improve the top of the funnel:** Test creative, messaging, targeting, offers, and calls-to-action to improve CTR.
2. **Scale selectively:** Increase investment gradually in campaigns combining strong ROI, conversion performance, and engagement.
3. **Optimize mixed performers:** Investigate campaigns with high revenue but low ROI, or high CTR but weak conversion.
4. **Review loss-making campaigns:** Validate data and business context before pausing or discontinuing negative-ROI campaigns.
5. **Refine audience and language strategy:** Use observed patterns to design targeted follow-up campaigns.
6. **Test channel strategies:** Validate channel findings before making major budget decisions.
7. **Run A/B tests:** Compare creative, language, offer, audience, or call-to-action variants. Track conversion rate as the primary metric and CTR, CPA, ROI, and revenue as supporting metrics.

## Suggested Power BI Dashboard
- **Executive Overview:** Revenue, spend, ROI, conversions, CTR, and conversion rate.
- **Funnel Analysis:** Stage volumes, conversion rates, and drop-offs.
- **Campaign Performance:** ROI, revenue, spend, and conversion rate by campaign.
- **Customer Segmentation:** Performance by target audience and customer segment.
- **Channel & Language:** Channel and language comparisons.
- **Spend Efficiency:** Spend vs ROI, spend vs revenue, high-ROI/low-spend campaigns, and high-revenue/low-ROI campaigns.

## Tools and Technologies
- Python, Pandas, NumPy
- Plotly and Matplotlib
- Jupyter Notebook / Google Colab
- Power BI
- SQL (where used in the workflow)

## Suggested Repository Structure
```text
Nykaa-Marketing-Campaign-Analysis/
├── data/
│   └── marketing_campaign_data.csv
├── notebooks/
│   └── nykaa_campaign_analysis.ipynb
├── dashboard/
│   └── nykaa_marketing_dashboard.pbix
├── report/
│   └── Nykaa_Marketing_Campaign_Analysis_Report.docx
├── presentation/
│   └── Nykaa_Marketing_Campaign_Analysis_Presentation.pptx
├── README.md
└── requirements.txt
```
Update example filenames to match the files you actually upload. Avoid uploading confidential or restricted data.

## Limitations
- The analysis is observational; correlation does not establish causation.
- Multi-channel campaigns make individual-channel attribution difficult.
- The dataset does not provide randomized control and treatment groups for causal A/B testing.
- Findings should be validated with business context before major budget decisions.
- Confirm metric definitions and units against the original dataset before publishing results.

## Conclusion
The analysis suggests Nykaa can improve marketing efficiency by **spending smarter, not simply spending more**. The largest funnel opportunity is converting impressions into clicks. Strong-performing campaign types, audience segments, languages, and channels provide directions for further investigation, while inefficient campaigns should be reviewed using ROI, conversion, engagement, and revenue together.

**Recommended approach:** Improve the top of the funnel → scale efficient campaigns carefully → refine audience and channel strategy → validate changes through controlled experiments.

## Author
**Harshita Tantia**  
Data Analytics Portfolio Project

`Python` · `Pandas` · `Plotly` · `SQL` · `Power BI` · `Marketing Analytics` · `Business Analytics`
