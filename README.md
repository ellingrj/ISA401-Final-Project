# ISA401 Final Project
This repository contains the final project for Miami's ISA401 class for Group 5.
Members: Rylee Elling, Lauren Gentile, Sophia Guibord, and Claire Kuzak.

# Our Project: How do advertisements influence the success of a streaming service?
This project investigates a central question in today’s media landscape:
How do advertisements influence the success of a streaming service?

As streaming platforms increasingly adopt ad‑supported models, understanding the relationship between ad load, ad spending, user engagement, and platform performance has become essential. To explore this, we compiled data from six different sources, consolidated them into a unified dataset, and analyzed cross‑platform patterns to uncover meaningful insights.

Our goal was to determine how advertising contributes to a platform’s revenue, viewership, subscriber base, and overall market presence.

# Data Sources
The dataset integrates metrics from industry reports and advertising analytics sources. Below is a breakdown of each platform and the data pulled from it.

[InsiderMonkey – 15 Biggest Streaming and TV Companies in the US (2022)](https://www.insidermonkey.com/blog/15-biggest-streaming-and-tv-companies-in-the-us-1192787/) and [InsiderMonkey - 5 biggest Streaming and TV Companies in the US](https://www.insidermonkey.com/blog/5-biggest-streaming-and-tv-companies-in-the-us-1192786/)

Data used:
- Estimated 2022 revenue for major streaming platforms.



[Brandience – Why Video Streaming Ads Are the Next Big Opportunity for Digital Marketers](https://brandience.com/insights/why-video-streaming-ads-are-the-next-big-opportunity-for-digital-marketers)

Data used:
- Estimated number of U.S. subscription OTT video viewers.



[AdTechRadar – Hulu, Amazon, Peacock Top Streaming Ad Spend Rankings; Table from EMARKETER Top 10 US Streaming TV Platforms, Ranked by Ad Spending, 2024 & 2025](https://adtechradar.com/2026/04/07/streaming-ad-spend-hulu-netflix-peacock-emarketer/)

Data used:
- 2024 ad spending by platform.
- 2025 ad spending by platform.
- Year‑over‑year ad spending percentage change.


[ElectroIQ – Streaming Services Statistics](https://electroiq.com/stats/streaming-services-statistics/)

Data used:
- Total global paid subscribers for each streaming service.


[The Streamable - Which streaming services are best, worst when it comes to ads?](https://thestreamable.com/how-many-ads-does-each-streaming-service-show)

Data used:
- Minimum and maximum ad minutes (movies and TV).
- Minimum and maximum ad break lengths (movies and TV).
- Presence of pre‑roll ads (movies and 30‑minute episodes).
- Minimum and maximum number of ad breaks (movies and 30‑minute episodes).


[Statista – Average Daily Time Watching Selected Video Streaming Services in the U.S. (2025)](https://www.statista.com/statistics/1610005/daily-time-spent-video-streaming/)

Data used:
- Average daily watch time for active users.
- Average daily watch time for all U.S. adults.



# Project Workflow

1. Data Collection: 
We gathered raw data from eight independent sources, each providing different metrics related to:
- Revenue
- Subscribers
- Ad spending
- Ad load and break structure
- Watch time

2. Data Cleaning: 
To merge the datasets, we:
- Standardized units (e.g., millions, percentages, minutes, seconds)
- Normalized platform names across sources
- Handled missing values (e.g., untracked ad spend)

3. Data Validation: 
To ensure all of our data was valid we checked: 
  - Data types make sense
  - No duplicate or misamed platform names
  - Numeric ranges are plausible (All mins < maxes, % change is accurate, watch time is reasonable, etc)
  - Missing values do not limit the analysis

4. Dataset Integration: 
All variables were combined into a single structured dataset, enabling cross‑platform comparisons and correlation analysis. The final dataset included 15 different platforms and 22 different metrics. 

View our presentation on the technical aspects of this project [here](https://www.youtube.com/watch?v=DyNn4ho0vrg).

5. Exploratory Data Analysis: 
We examined...
- Revenue to identify the top performing streaming services.
- Ad Spending By Subscriber By Platform for our top performers to analyze ad spending and how it relates to success via subscriptions.
- Engagement Score By Platform for our top performers to analyze ad effects on engagement from users.
- Watch Time vs Max Number of Ads for TV episodes to view how often ads are being playing in a single episode. 

7. Insight Generation: 
Using visualizations and statistical summaries [created in Tableau](https://public.tableau.com/shared/DSYTFDNGX?:display_count=n&:origin=viz_share_link), we developed insights into:
- Engagement score: Netflix dominates engagement by a significant margin, having an average score of 11,605 while other platforms like Hulu, Amazon Prime, and Disney+ hold steady in the middle, and HBO Max and Peacock are falling behind. This reveals that a larger subscriber base does not always correlate with stronger viewer engagement. Platforms with lower scores struggle to justify premier ad rates, regardless of how many subscribers they may have. 


- Revenue Per Platform: Netflix is the leader with almost $32 billion in revenue. Although Amazon Prime Video is the second largest revenue streaming platform, Netflix still has almost double their revenue, making it a clear dominating platform compared to its top competitors in the market. The market is highly concentrated by the top 4 highest revenue platforms, Netflix, Amazon Prime Video, Disney+, and HBO Max, leaving smaller platforms relying on possible segmented aspects like bundles, provider support, or niche audiences.

- Ad Spending By Subscriber Count By Platform: Hulu is shown to have the most ad spend, despite not having the largest subscriber count. This can potentially explain that Hulu is investing in market expansion. Netflix has the largest subscriber count, while having almost the lowest ad spend. This shows that the highest ad spend does not always mean the most subscribers, it truly comes down to brand loyalty. 

- Watch time vs. Max number of Ads: The data reveals a clear inverse correlation between ad density and user retention. Platforms that maintain low interruption levels, for example, Netflix at 2 minutes, achieve peak engagement exceeding 60 minutes daily. Conversely, when ad loads cross the 7-minute threshold, daily watch time drops significantly, with Disney+ hitting a saturation point at 10 minutes of ads per episode. 

