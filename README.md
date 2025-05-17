# MARKETING-CAMPAIGN-PERFORMANCE-ANALYSIS-USING-SQL
Analyzed a marketing dataset using SQL to uncover key performance insights, including impressions, ROI, CTR, and user engagement. I also documented queries and findings to support data-driven decisions for campaign optimization

Table of content

- [Introduction](https://github.com/Ehinmetan/MARKETING-CAMPAIGN-PERFORMANCE-ANALYSIS-USING-SQL#introduction)

- [Objectives](https://github.com/Ehinmetan/MARKETING-CAMPAIGN-PERFORMANCE-ANALYSIS-USING-SQL/blob/main/README.md#objectives)

- [Data overview and Data Structure](https://github.com/Ehinmetan/MARKETING-CAMPAIGN-PERFORMANCE-ANALYSIS-USING-SQL/blob/main/README.md#data-overview-and-dataset-structure)

- [Data Structure](https://github.com/Ehinmetan/MARKETING-CAMPAIGN-PERFORMANCE-ANALYSIS-USING-SQL/blob/main/README.md#dataset-structure)

# Introduction
In today’s digital landscape, marketing campaigns play a pivotal role in shaping brand visibility, driving customer engagement, and ultimately increasing conversions. Companies invest heavily in online advertising, leveraging various channels such as Google Ads, social media, email marketing, and influencer partnerships to reach their target audiences. However, not all campaigns deliver the desired results, some generate significant traction, while others underperform, leading to inefficient spending and lost opportunities.

# Objectives
This study focuses on analyzing a marketing campaign dataset using Structured Query Language (SQL) to extract actionable insights. By running targeted SQL queries, we aim to:
- Identify the campaigns with the highest impressions to assess audience reach.
  
- Determine which campaign delivered the highest ROI, helping businesses allocate budgets more effectively.
  
- Analyze top-performing locations to guide regional marketing strategies.
  
- Evaluate the average engagement score by target audience, ensuring marketing efforts are tailored to responsive demographics.
 
- Calculate the overall Click-Through Rate (CTR) to measure how well ads convert views into interactions.
  
- Find the most cost-effective campaigns, ensuring optimized ad spend.
  
- Rank marketing channels by total conversions, highlighting the most effective platforms for future investment.
  

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

- **Total Impressions for Each Campaign**: This analysis calculates the total number of impressions for each campaign. It helps measure the reach of different campaigns and assess their visibility.
  
![1](https://github.com/user-attachments/assets/8d38a999-f502-4ba0-aa65-259cd7c7dd54)

![2 sqlPicture](https://github.com/user-attachments/assets/c6df4299-324f-4f69-b000-db91a63c8752)

 **Key Findings**: The total impressions analysis showed that campaigns varied widely in their reach, with some significantly outperforming others in terms of visibility.
 
- **Campaign with the Highest ROI**: This analysis identifies the campaign with the highest return on investment (ROI). It provides insights into which campaign delivered the most value relative to its cost.
  
  ![2](https://github.com/user-attachments/assets/8daef720-eac4-4a97-abab-0bd1988b5e0a)

  ![OUT2](https://github.com/user-attachments/assets/58562cbf-28c6-4cae-896d-7014dddeb49f)
  
  **Key Findings**: The analysis identified Campaign ID 168 from NexGen Systems as the campaign with the highest return on investment (ROI), achieving a value of 8.00. This indicates that NexGen Systems' campaign generated the highest profitability relative to its cost, making it the most successful in terms of returns.

  - **Locations with the Most Impressions**: This analysis determines the locations that generated the highest number of ad impressions. It helps in understanding where the advertisements gained the most visibility.

![3](https://github.com/user-attachments/assets/6d177b04-66d3-474d-922c-f8bd4ba70a18)

![OUT 3](https://github.com/user-attachments/assets/19929e95-d73a-41d3-a032-ecf1d146eddc)

  **Key Findings**: The analysis showed that New York recorded the highest number of ad impressions (22,135,9756), followed closely by Miami (22,134,7726) and Chicago (21,999,9352). This indicates strong marketing exposure in these cities, positioning them as strategic targets for focused advertising efforts.

- **Average Engagement Score for Target Audience**: This analysis calculates the average engagement score for different audience segments. It helps assess how effectively each audience interacts with the campaign content.

![4](https://github.com/user-attachments/assets/2b2fa9cc-e5a9-46b8-98f5-10a7f195227b)

![OUT4](https://github.com/user-attachments/assets/0dd2020f-01d8-46d6-ab9a-2b7c672ca06d)

  **Key Findings**: Men aged 18–24 recorded the highest engagement score (5.51), indicating the strongest interaction with marketing content. Other high-performing segments included Men 25–34 and Women 25–34, each with engagement scores above 5.49. This highlights young adults as a highly responsive demographic for current campaigns.

 - **Overall Click-Through Rate (CTR)**:This metric reflects how effectively the marketing campaigns convert impressions into clicks, serving as a key indicator of audience engagement with the ads.

![5](https://github.com/user-attachments/assets/f0c9bea7-3049-40b5-98c4-b89fd28ec9c3)

![OUT5](https://github.com/user-attachments/assets/3ddd179e-4141-48c2-aa58-791890b9400d)

**Key Findings**: The overall Click-Through Rate (CTR) across all campaigns was 9.98%, reflecting strong user engagement. A high CTR indicates that the ads effectively captured attention and prompted action.

- **Most Cost-Effective Campaign**: This analysis identifies the campaign with the lowest cost per conversion. It helps in evaluating which  campaign delivers the best results at the least expense.

![6](https://github.com/user-attachments/assets/dd4f885b-9f37-4dfa-9f95-55867323a766)

![OUT6](https://github.com/user-attachments/assets/f697f6c1-169d-4487-b863-1179edc1ec54)

**Key Findings**: Alpha Innovations ran the most cost-effective ampaign, with a cost per conversion of $33,346.67. This means that while their campaign converted leads effectively, the cost per acquired customer remains high.

- **High-Performing Campaigns (CTR > 5%)**: This analysis identified campaigns with a Click-Through Rate above 5%, spotlighting those with the strongest user engagement. Filtering by this threshold helps prioritize campaigns that are performing above average and may warrant additional investment

![7 sqlPicture](https://github.com/user-attachments/assets/c96fd584-b618-41de-903c-743f88ed8e22)

![7 output sql Picture](https://github.com/user-attachments/assets/c83b9e69-8d27-4fbc-a4fd-e531ac702460)

**Key Findings** The SQL query retrieved campaigns where CTR exceeded 5%, ensuring only highly engaging campaigns were considered. These  campaigns demonstrated superior audience interaction. 

- **Channel Performance by Conversions**: This analysis ranks marketing channels based on total conversions to identify the most impactful platforms. It provided clear insights into which channels are driving the most customer actions, helping to guide future budget allocation and campaign strategy.

![8](https://github.com/user-attachments/assets/82fb4d8b-ee81-4d5e-9089-a9b19d5d7eca)

![OUT 8](https://github.com/user-attachments/assets/c65cd1f0-1ad4-4fe7-b3d8-e36b026dff2d)

**Key Findings** The top-performing marketing channels based on total conversions are Email with 2,697.38 conversions, Google Ads with 2,681.24 conversions, Website with 2,674.95 conversions, YouTube with 2,667.76 conversions, Instagram with 2,667.57 conversions, and Facebook with 2,625.27 conversions. Email marketing generated 
the highest number of conversions, indicating that direct communication with users was the most effective channel.

# CONCLUSION
The analysis of the marketing campaign dataset provided several key insights that can guide future marketing decisions:

- **Campaign Reach**: The total impressions analysis showed thatcampaigns varied widely in their reach, with some significantly outperforming others in terms of visibility.

• **Most Profitable Campaign**: Campaign ID 168 from NexGen Systems had the highest return on investment (ROI) at 8.00, making it the most profitable marketing effort.

- **Top Locations for Impressions**: New York (22,135,9756), Miami (22,134,7726), and Chicago (21,999,9352) were identified as the cities with the highest number of impressions, making them prime locations for targeted advertising.

- **Audience Engagement**: The highest engagement score was observed among Men aged 18-24 (5.51), indicating strong responsiveness to marketing efforts. Men 25-34 and Women 25-34 also demonstrated high engagement levels.

- **Campaign Effectiveness**: The overall click-through rate (CTR) for all campaigns was 9.98%, demonstrating strong user interaction with advertisements.

- **Cost Efficiency**: Alpha Innovations led in cost efficiency, with the lowest cost per conversion at $33,346.67, though the absolute cost remained high.

- **High-Performing Campaigns**: Campaigns exceeding a 5% CTR threshold were identified, ensuring that the most engaging campaigns were highlighted.

- **Best Performing Marketing Channels**: Email marketing generated the highest number of conversions (2,697.38), followed closely by Google Ads (2,681.24) and the Website channel (2,674.95), showing the effectiveness of direct communication and digital advertising.

These insights provide a data-driven foundation for optimizing future marketing campaigns, focusing on high-performing demographics, locations, and channels while improving cost efficiency and engagement strategies.

# RECOMMENDATIONS
To enhance marketing performance and cost-effectiveness:

- **Prioritize High-Performing Locations**: Focus marketing efforts  in New York, Miami, and Chicago.

- **Replicate High-ROI Campaign Tactics**: Analyze and adopt strategies from NexGen Systems, whose campaigns demonstrated strong returns on investment.

- **Target Young Adult Demographics**: Develop tailored content for 18–34-year-olds, especially men aged 18–24, who showed the highest engagement scores.

- **Increase Email Marketing Investment**: Expand personalization and automation to sustain high conversion rates.

- **Improve Cost Efficiency**: Reevaluate ad spending to reduce customer acquisition costs without sacrificing performance.

- **Refine Strategies Using High-CTR Campaigns**:Use insights from top-performing campaigns (CTR > 5%) to sharpen messaging and creative direction.

 - **Diversify Channel Strategy**:
Maintain a balanced marketing mix by continuing investments across email, Google Ads, and website campaigns to spread risk and reach.

 
