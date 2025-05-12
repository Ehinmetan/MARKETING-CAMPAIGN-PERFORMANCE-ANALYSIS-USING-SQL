# MARKETING-CAMPAIGN-PERFORMANCE-ANALYSIS-USING-SQL
Analyzed a marketing dataset using SQL to uncover key performance insights, including impressions, ROI, CTR, and user engagement. I also documented queries and findings to support data-driven decisions for campaign optimization

# Introduction
In today’s digital landscape, marketing campaigns play a pivotal role in shaping brand visibility, driving customer engagement, and ultimately increasing conversions. Companies invest heavily in online advertising, leveraging various channels such as Google Ads, social media, email marketing, and influencer partnerships to reach their target audiences. However, not all campaigns deliver the desired results; some generate significant traction, while others underperform, leading to inefficient spending and lost opportunities.

This study focuses on analyzing a marketing campaign dataset using Structured Query Language (SQL) to extract actionable insights. By running targeted SQL queries, we aim to:
- Identify the campaigns with the highest impressions to assess audience reach.
  
- Determine which campaign delivered the highest ROI, helping businesses allocate budgets more effectively.
  
- Analyze top-performing locations to guide regional marketing strategies.
  
- Evaluate the average engagement score by target audience, ensuring marketing efforts are tailored to responsive demographics.
 
- Calculate the overall Click-Through Rate (CTR) to measure how well ads convert views into interactions.
  
- Find the most cost-effective campaigns, ensuring optimized ad spend.
  
- Rank marketing channels by total conversions, highlighting the most effective platforms for future investment.
  
By answering these questions, this analysis will provide valuable insights that help marketers make data-driven decisions, optimize campaign strategies, and improve overall marketing efficiency. Businesses can use these findings to fine-tune ad placements, enhance audience targeting, and maximize conversion potential, ensuring higher profitability and reduced wasted ad spend.
# Data Overview and Dataset Structure

To effectively analyze the performance of marketing campaigns, we use a structured dataset containing key performance indicators (KPIs) and campaign-specific attributes. This dataset enables businesses to evaluate engagement levels, cost efficiency, and overall campaign effectiveness, helping them optimize future marketing strategies.
## Key Variables
The dataset captures crucial details about various marketing campaigns, including company information, advertising channels, and financial performance metrics. Below is a breakdown of the key variables:

**Campaign Details**

- **Campaign_ID (Integer)**: A unique identifier assigned to each campaign. (Primary Key)
  
- **Company (String)**: The name of the company running the campaign.
  
- **Campaign_Type (String)**: Specifies the type of marketing campaign (e.g., Email, Display, Influencer).
  
- **Duration (String)**: The total length of the campaign (e.g., "30 days").
  
- **Channel_Used (String)**: The platform where the campaign was executed (e.g., Google Ads, YouTube).
  
**Performance Metrics**

- **Impressions (Integer)**: The total number of times the advertisement was displayed to users.
  
- **Clicks (Integer)**: The number of times users clicked on the advertisement.
  
- **Engagement_Score (Integer)**: A score (ranging from 1 to 10) that measures user interaction and engagement with the campaign.
  
- **Conversion_Rate (Float)**: The percentage of users who took a desired action (e.g., purchase, sign-up) after interacting with the campaign.
  
**Financial Metrics**

- **Acquisition_Cost (Float)**:  The cost incurred by the company to acquire a new customer through the campaign.
  
- **ROI (Return on Investment) (Float)**: A profitability metric that measures the effectiveness of a campaign relative to its cost.
  
**Geographic Targeting**

- **Location (String)** – The geographic region where the campaign was targeted.

  # Dataset Structure
The dataset is structured in a tabular format, where each row represents a unique marketing campaign. This ensures that the dataset maintains data integrity and uniqueness while enabling efficient querying and analysis.

**Data Organization:**

- The primary key is Campaign_ID, ensuring each campaign is uniquely identifiable.

- Categorical variables include Company, Campaign_Type, Channel_Used, and Location.
  
- Numerical variables (e.g., Impressions, Clicks, Conversion_Rate, ROI) capture key performance metrics.
  
- The dataset is optimized for SQL-based queries, allowing for easy filtering, aggregation, and performance analysis.
  
This structured format enables efficient data retrieval for insights related to campaign performance, audience engagement, and cost-effectiveness. By leveraging SQL queries, we can uncover trends, rank top-performing campaigns, and optimize marketing spend. 

# SQL Queries and Analysis
This section provides a detailed breakdown of the SQL queries used to analyze the dataset, along with the methods, results, insights, and visual representations.

**Total Impressions for Each Campaign**
