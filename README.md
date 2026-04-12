# Cyclistic Rider Behaviour Intelligence Dashboard (Casual-to-Member Conversion Analysis) 

## 1. Executive Summary
This project analyzes Cyclistic bike-share data to uncover key behavioural differences between casual riders and annual members, with the goal of supporting data-driven customer conversion strategies.

Using cleaned and structured ride data, the analysis focuses on usage patterns such as ride frequency, duration, time of day, and day-of-week trends to identify how each customer segment interacts with the service.

The core business problem addressed is the lack of clear insight into how casual riders behave compared to members, limiting the company’s ability to design effective marketing and conversion strategies.

The key outcome of this project is a set of actionable insights showing that casual riders are more leisure-oriented (longer rides, weekend usage), while members exhibit consistent, commute-driven behaviour. These insights provide a strong foundation for targeted strategies aimed at converting high-potential casual users into long-term subscribers.

## 2. Project Overview
This project is set in the urban mobility and bike-share industry, where recurring memberships drive stable revenue.

Cyclistic Bike-Share operates in a competitive market where annual members generate more long-term value than casual riders, who use the service inconsistently.

However, the company lacks clear insight into how these two groups differ in behaviour and usage, limiting its ability to design effective conversion strategies.

This project addresses that gap by transforming raw ride data into structured insights, identifying key behavioural differences and uncovering opportunities to convert high-potential casual riders into long-term members.

## 3. Data Source
### 3.1 Dataset Description

The dataset used for this analysis was sourced from the Cyclistic Bike-Share historical trip data, made available for analysis as part of a public case study dataset.

It contains detailed ride-level information capturing how users interact with the bike-share system across different time periods.

### 3.2 Data Structure

The raw dataset consisted of:

* 5,552,994 rows (individual ride records)
* 13 columns (ride attributes and user details)

Key Variables Include:

* ride_id
* rideable_type
* started_at 
* ended_at
* start_station_name 
* end_station_name
* start_lat 
* start_lng
* end_lat 
* end_lng
* member_casual

The data includes a mix of:

* Categorical variables (e.g., rideable_type, member_casual)
* Datetime variables (e.g., started_at, ended_at)
* Numerical variables (e.g., latitude, longitude)
  
### 3.3 Data Scope
- The data covers multiple months of ride activity
- The data represents real-world usage patterns of Cyclistic Bike-Share users
- The data is focused on urban mobility behaviour within a single city environment (Chicago)

### 3.4 Data Limitations

* Missing Values: Some station names and location fields contained null values
* No Demographics: No user-level data (age, gender, income), limiting deeper segmentation
* External Factors Excluded: Weather, events, and traffic conditions were not included
* Data Quality Issues: Required cleaning for inconsistencies and invalid ride durations
  
## 4. Problem Statement

**What is the problem?**

Cyclistic Bike-Share aims to increase the number of annual members but lacks clear insight into how casual riders differ from members in terms of behaviour and usage patterns.

Without this understanding, it is difficult to identify which casual users are most likely to convert and how to effectively target them.

**Why is it important?**
* Revenue Growth: Annual members provide more consistent and predictable revenue compared to casual riders
* Customer Retention: Converting casual users improves long-term customer value
* Marketing Efficiency: Data-driven insights enable more targeted and cost-effective campaigns

**Key Questions**
* Behaviour Gap: How do casual riders differ from members in terms of ride frequency and duration?
* Time Patterns: When do each user group ride (time of day, day of week)?
* Usage Intent: Are casual riders primarily leisure-based while members are commute-driven?
* Conversion Opportunity: Which behavioural patterns indicate a higher likelihood of converting casual riders into annual members?

## 5. Tools & Methodology

**Tools Used**
* Python: Data cleaning, preprocessing, and transformation
* Power BI: Data modelling, analysis, and dashboard development
* PowerPoint (Optional): Wireframing and dashboard layout planning
  
### Methodology

**I. Data Collection**

The dataset was provided by Motivate International Inc. as part of the Google Data Analytics Capstone Project. It contains historical trip data representing real-world user activity.

**II. Data Cleaning & Preparation**
* Removed duplicate records
* Handled missing and null values
* Standardized date-time formats
* Filtered out invalid or unrealistic ride durations

III. Data Transformation & Processing
* Converted raw datetime fields into structured formats
* Created derived features such as ride length in minutes 
* Prepared data for analysis by ensuring consistency across all records
  
**IV. Feature Engineering (Calculated Fields)**
* Calculated Column (Date): Extracted date from timestamp for trend analysis
* Custom Column (Hour): Derived hour of ride to analyze time-of-day patterns

**V. Data Validation**
* Verified data consistency after cleaning and transformation
* Cross-checked key metrics (e.g., ride duration, counts) for accuracy

**VI. Data Modelling**
* Structured the dataset within Power BI to support efficient querying and analysis
* Ensured relationships and data types were correctly defined for reporting

**VII. Data Visualization**
* Built an interactive Power BI dashboard
* Designed a homepage for intuitive navigation
* Developed visuals to highlight behavioural differences between user segments

## 6. Exploratory Data Analysis (EDA)

The exploratory analysis focused on identifying key behavioural patterns between casual riders and annual members, with emphasis on usage trends, ride duration, and time-based activity.

**I. Ride Frequency Patterns**

Clear differences were observed in ride frequency across user types.

* Casual riders show higher activity during weekends
* Members exhibit consistent usage throughout weekdays

This indicates a distinction between leisure-based usage and routine/commute-driven behaviour.

**II. Time-Based Trends**

Time-of-day analysis revealed distinct usage patterns:

* Members peak during morning and evening hours, aligning with work commutes
* Casual riders are more active during midday and afternoon periods

This reinforces the difference in usage intent between both groups.

**III. Ride Duration Distribution**

A significant gap exists in ride duration:

* Casual riders tend to take longer rides on average
* Members typically take shorter, more frequent trips

This suggests casual users prioritize experience, while members prioritize efficiency.

**IV. Weekly Usage Trends**
* Weekend usage is dominated by casual riders
* Weekday usage is driven primarily by members

This pattern highlights strong behavioural segmentation based on time.

**V. Outliers & Data Observations**
Some rides showed unusually long durations, indicating potential anomalies or extended leisure trips
These outliers were reviewed during the data cleaning stage to ensure they did not distort analysis results

## 7. Key Insights

The analysis revealed clear behavioural differences between casual riders and annual members, highlighting strong opportunities for targeted conversion strategies.

### Insight 1: High Proportion of Casual Riders

**What happened?**
Casual riders account for 55.04% of total rides, while members make up 44.96%.

**Why did it happen?**
A large portion of users engage with the service without committing to membership, likely due to occasional or leisure-based usage patterns.

**Why does it matter?**
This represents a significant untapped opportunity. Converting even a fraction of casual riders into members could substantially increase recurring revenue.

### Insight 2: Ride Duration Gap

**What happened?**
Casual riders have a higher average ride duration (17.64 minutes) compared to members (12.9 minutes).

**Why did it happen?**
Casual riders are more leisure-oriented, taking longer trips, while members use bikes for shorter, routine activities such as commuting.

**Why does it matter?**
High-engagement casual riders (longer trips) are strong candidates for membership conversion, as they already derive more value from the service.

### Insight 3: Weekly Usage Patterns

**What happened?**
Casual riders peak on weekends (Saturday and Sunday), while members are more active during weekdays, especially midweek.

**Why did it happen?**
Casual riders use bikes primarily for recreation, while members rely on them for structured, weekday routines like commuting.

**Why does it matter?**
Weekend-focused campaigns and promotions can effectively target casual riders when engagement is highest, increasing conversion potential.

### Insight 4: Time-of-Day Behaviour

**What happened?**
Casual riders are most active in the late afternoon and evening (3 PM – 7 PM), while members peak during commute hours (4 PM – 6 PM).

**Why did it happen?**
Casual usage aligns with free time after work or school, whereas member usage reflects structured daily schedules.

**Why does it matter?**
Timing promotions during peak casual usage hours (especially evenings) can significantly improve visibility and engagement for conversion campaigns.

### Insight 5: Bike Preference Among Casual Riders

**What happened?**
A majority of casual riders (56.67%) prefer electric bikes over classic bikes (43.33%).

**Why did it happen?**
Electric bikes offer convenience and ease of use, making them more attractive for leisure and longer rides.

**Why does it matter?**
Highlighting electric bike benefits in marketing campaigns or offering incentives tied to their usage can increase appeal and drive membership conversions.

### Insight 6: High-Traffic Stations for Casual Riders

**What happened?**
Casual riders are concentrated around specific stations, including high-traffic locations such as Milwaukee Ave & Ainslie St and Portage Park.

**Why did it happen?**
These stations are likely located near recreational areas or accessible neighborhoods that attract leisure riders.

**Why does it matter?**
These locations present strategic touchpoints for targeted marketing—such as on-site promotions, discounts, or trial memberships—to convert casual riders at the point of highest engagement.

## 8. Visuals Preview


**Visual Type 1: Annotated Dashboard Screenshots**

<img width="1101" height="485" alt="Screenshot 2026-04-07 082042" src="https://github.com/user-attachments/assets/5a80c071-6710-46f2-b71e-a2c852493853" />

**Visual Type 2: Data Cleaning (Before vs After)**

*Excerpt of Uncleaned Dataset*
<img width="1133" height="181" alt="Screenshot 2026-04-10 004643" src="https://github.com/user-attachments/assets/3e490a4c-55a2-40f9-a07f-a45148d679de" />

*Excerpt of Uncleaned Dataset*
<img width="1115" height="166" alt="Screenshot 2026-04-10 004730" src="https://github.com/user-attachments/assets/5f02b097-7bba-46b6-984a-9d54e7203781" />



**Visual Type 3: Python Code Snippets**

*Data Cleaning Pythn code snippet*
<img width="1057" height="445" alt="Screenshot 2026-04-10 005434" src="https://github.com/user-attachments/assets/b6ecb85f-85b8-43ee-841e-20bf4b8be1a2" />

*Data Analysis Python Code Snippet*
<img width="703" height="459" alt="Screenshot 2026-04-10 005619" src="https://github.com/user-attachments/assets/ee709fc8-b755-4705-b98a-582dc22f533b" />

Full implementation is available in the project repository.



**Visual Type 5: Process Flow Diagram**

<img width="340" height="405" alt="Screenshot 2026-04-10 011510" src="https://github.com/user-attachments/assets/bb3618f7-d91d-4adb-b111-85376de7b943" />


Description:

This diagram outlines the end-to-end workflow of the project, from data collection to visualization. It reflects the structured methodology used to transform raw data into actionable insights.

## 9. Strategic Recommendations

Based on the identified behavioural patterns, the following strategies are recommended to increase conversion of casual riders into annual members:

**1. Target High-Value Casual Riders (Long-Duration Users)**

Casual riders have significantly longer average ride durations, indicating higher engagement with the service.

Recommendation:
Introduce personalized membership offers for users with longer ride durations, such as discounted trial memberships or ride credits after a usage threshold.

Expected Impact:
Converts high-usage casual riders who already derive strong value, increasing membership adoption and long-term revenue.

**2. Weekend-Focused Conversion Campaigns**

Casual rider activity peaks on weekends, particularly Saturday and Sunday.

Recommendation:
Launch targeted marketing campaigns during weekends, including:

Limited-time membership discounts
Weekend-only promotions
In-app notifications during peak periods

Expected Impact:
Maximizes visibility and engagement when casual riders are most active, improving conversion rates.

**3. Time-Based Engagement Strategy**

Casual riders are most active in the late afternoon and evening (3 PM – 7 PM).

Recommendation:
Deploy time-sensitive promotions during peak hours, such as:

“Ride more, save more” offers
Evening membership incentives
Push notifications during high-traffic periods

Expected Impact:
Increases the likelihood of conversion by engaging users at the point of highest activity.

**4. Leverage Electric Bike Preference**

A majority of casual riders prefer electric bikes, indicating a strong preference for convenience and ease of use.

Recommendation:
Position electric bikes as a key benefit of membership by:

Offering exclusive discounts on electric bike rides for members
Providing free or discounted trials for electric bike usage

Expected Impact:
Aligns membership value with user preferences, making the upgrade more attractive.

**5. Location-Based Marketing at High-Traffic Stations**

Casual riders are concentrated around specific high-traffic stations.

Recommendation:
Deploy targeted marketing at these locations through:

On-site promotions and signage
QR codes for instant membership sign-up
Localized campaigns or events

Expected Impact:
Captures users at the point of highest engagement, increasing conversion opportunities.

**6. Introduce Flexible Membership Options**

The behavioural gap between casual and member usage suggests that some users may not be ready for full annual commitments.

Recommendation:
Introduce flexible plans such as:

* Monthly or pay-as-you-go memberships
* Trial membership periods
* Tiered pricing options

Expected Impact:
Reduces entry barriers and encourages gradual transition from casual usage to full membership.


## 10. Limitations & Assumptions

While this project provides valuable insights into rider behaviour and conversion opportunities, it is subject to several limitations and assumptions:

* Missing values were present in key fields and removed during data cleaning
* Some records with unrealistic ride durations were excluded based on logical assumptions
* The dataset does not include demographic information such as age, gender, or income
* External factors like weather, events, and traffic were not considered
* The analysis is limited to a single city (Chicago)
* Behavioural interpretations are inferred from patterns and not directly validated
* The dataset covers a limited time period and may not reflect long-term trends


## 11. Implementation Plan

This section outlines how the insights from this analysis can be translated into actionable strategies to increase conversion of casual riders into annual members.

**What Needs to Be Done**
* Launch targeted marketing campaigns focused on high-engagement casual riders
* Introduce flexible membership plans and trial offers
* Deploy time-based and location-based promotions
* Highlight electric bike benefits in membership messaging
  
**Who is Responsible**
* Marketing Team: Campaign design, promotions, and customer targeting
* Product Team: Membership plans, pricing structure, and feature updates
* Data Team: Ongoing analysis, user segmentation, and performance tracking
* Operations Team: On-ground execution at high-traffic stations
  
**When Should It Happen**
* Weekend campaigns (Friday evening – Sunday)
* Peak hours (3 PM – 7 PM)
* Seasonal high-demand periods (spring/summer months)
  
**How Will Success Be Measured**
* Increase in casual-to-member conversion rate
* Growth in membership sign-ups
* Improvement in user retention rates
* Engagement metrics (click-through rates, promotion usage)
  
**Resources Required**
* Marketing budget for campaigns and promotions
Product development support for new membership options
Data infrastructure for tracking and analysis
On-ground materials (QR codes, signage at stations)

**Potential Risks & Challenges**
* Low conversion despite high engagement
* Ineffective targeting of casual riders
* Operational challenges in campaign execution
* External factors (weather, seasonality) affecting results

## 12. Conclusion

This project addressed the challenge of converting casual riders into annual members by analyzing behavioural differences within the Cyclistic bike-share system.

The analysis revealed clear patterns: casual riders are more leisure-oriented, ride longer, prefer weekends, and show strong interest in electric bikes, while members exhibit more consistent, commute-driven behaviour.

These insights highlight a significant opportunity for targeted conversion strategies. By aligning marketing efforts, pricing models, and product offerings with actual user behaviour, Cyclistic can effectively increase membership adoption, improve customer retention, and drive more stable, long-term revenue growth.


## 13. Table of Contents
1. [Executive Summary](#1-executive-summary)
2. [Project Overview](#2-project-overview)
3. [Data Source](#3-data-source)
4. [Problem Statement](#4-problem-statement)
5. [Tools & Methodology](#5-tools--methodology)
6. [Exploratory Data Analysis (EDA)](#6-exploratory-data-analysis-eda)
7. [Key Insights](#7-key-insights)
8. [Visuals Preview](#8-visuals-preview)
9. [Strategic Recommendations](#9-strategic-recommendations)
10. [Limitations & Assumptions](#10-limitations--assumptions)
11. [Implementation Plan](#11-implementation-plan)
13. [Conclusion](#12-conclusion)
