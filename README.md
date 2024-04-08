# Uniace-Traffic-analysis
Uniace - an online learning platform had some interactive data of users. The goals of this analysis were to get insights about users, which courses they accessed the most, and which Referrer brought them to the website.

I. Data from table Uniace.csv:
- email: user email
- type: interactive data. ex: click, open, unsubscribe, page
- name: course name
- MA URL: URL 
- MA_Referrer: referrer url
- IP Address
- Date: The date that the customer interacted with the website

II. Steps:  
  1. ETL Data and Data Analysis
    - 1.1. Load and combine multiple data files into a big data file
    - 1.2. Data preprocessing: Rename, Change data type, fill null cells,
    - 1.3. Split the email to get the email domain. From the email domain, categorize customers into different groups: Work (if the domain contains Outlook), Student (if the domain contains edu), guest (if the domain is null), and other
    - 1.4. For Student users: using Regular Expression to map the school to their correct email domain
    - 1.5. From Referrer column, map the customer sources: Search Engine, Social Media, Organic, 3rd party, and other
    - 1.6. From IP Address column, map the customer geography: Vietnam, USA, Canada, Korea, Japan, ...
    - 1.7. From Course name column, map the topic: Data Analytics, Business Intelligence, Soft Skills, Programming Language, ...
    - 1.8. From Date column, retrieve Hour, DayOfWeek column to analyze the traffic by Hour and DayOfWeek
    - 1.9. Save the cleaned data into data warehouse and ready for further analysis
     

  2. Data Visualization
     - 2.1. Load data into Power BI desktop
     - 2.2. Calculate some metrics: TotalAccesses = COUNT(IPAddress); TotalUniqueAccesses = DISTINCTCOUNT(IPAddress), AvgAccessesPerUser = TotalAccesses / TotalUniqueAccesses
     - 2.3. Generate the Overview dashboard
     - 2.4. Generate the Detailed dashboard
         - 2.4.1. Visualize the top 3 countries with the most users
         - 2.4.2. Visualize Users by Category
         - 2.4.3. Visualize the Top 5 schools with the most users
         - 2.4.4. Analyze Users by Geography and Topics
         - 2.4.5. Analyze Users by Categories and Topics


III. Tools:
- Python: Pandas, os, re, matplotlib, seaborn, geopandas, plotly
- Power BI Desktop
