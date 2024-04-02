# Uniace-Traffic-analysis
Uniace - an online learning platform had some interactive data of users. The goals of this analysis were to get insights about users, which courses were they accessed the most, and which Referrer brought them to the website.

I. Data from table Uniace.csv:
- email: user email
- type: interactive data. ex: click, open, unsubscribe, page
- name: course name
- MA URL: url 
- MA_Referrer: referrer url
- ma_path: path url
- IP Address
- cuid: customer ID
- Date: Date that customer interacted with the website
- tag: tag of the course, category.

II. Steps:
  1. Load data into Power BI
     
  2. Data Processing and Data Analysis
     - 2.1. From email, retrived the email domain
     - 2.2. Every school/ company/ organization has their own domain, mapped those email domain with their school/ company/ organization
     - 2.3. Analyzed CustomerSource based on MA_Referrer. Customers might come from: 3rd Parties, android, Organic, Search engine, social media
     - 2.4. Retrived customer Geography based on the url. Ex: .vn = vietnam, .jp = japan, .uk = United Kingdom, ...
     - 2.5. Categorized customer into different groups: Work, student, or normal based on email domain
     - 2.6. Mapped the name (course name) to the appropriate topics: Data Science, Coding, Critical Thinking, Learning, ...
     

  3. Data Visualization
     - 3.1. Generated an overview Dashboard. Using basic statistics method: Min, Max, Average, Count, Sum, Group by
     - 3.2. Generated an detailed Dashboard.
         -3.2.1. Visualized customers by Geography, Category
         -3.2.2. Calculated Average accesses by Geography, customer Category and Topics
         -3.2.3. Summarized top 5 schools have the most accesses, and which topics are accessed the most

  4. Generate report
     - 4.1. Checked the shops with the most orders and most more-than-one-time orders with the max rebate
     - 4.2. Checked the users were trying to buy from the same shops and maxed out the rebate on every order
     - 4.3. Matched the results to see which shops were trying cooperate with users to took advantages of the promotion programs


III. Tools:
- Power BI Desktop
- PowerPoint
