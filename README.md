# 2Market-marketing-campaign
Through analysing a dataset from the previous campaign, we can recommend the most effective advertising channel to use.


Background
2Market are in the early stages of planning a new marketing campaign. Through
analysing a dataset from the previous campaign, we can recommend the most
effective advertising channel to use. Furthermore, having a better understanding of
customer demographics and best-selling products will help 2Market to develop an
advertising strategy to increase average product sales of target groups.
How will the effectiveness of advertising channel be measured?
What relationships can we find between demographics and products sales?
What products should be advertised?





Analytical Approach




Data cleaning processes began with changing column data types to correct format
(e.g., Number, Date), henceforth:
1. Age value was created using calculation from Birth Year.
2. Marital status contained several values not considered useful, these were
marked (#N/A) and consolidated using a lookup table e.g., “Alone” edited to
be “Single”.
3. Abbreviated country names were changed to full names for ease of
presenting.
4. New columns for Amount Total, Total Children and Total Ads created to allow
for easier analysis.
5. Marking outliers (see Fig. 1) and duplicates (see Fig. 2) for filtering.
Excel provided for basic analysis of the cleaned dataset beginning with Total
Customers (2005), Average Age (53.13), Average Income ($52,045) and Average
Sale (607.62). The most common demographics are identified as:
 Education: Graduates (1012), PhD (424)
 Marital Status: Together & Married (1289)
 Country: Spain (997), South Africa (300)
Using PivotTables to manipulate the data, charts were created showing demographic
trends. Fig. 3 illustrates the relationship between level of education, age and income,
the trend is a higher level of education will correlate with increased age and income.
Similarly, Fig. 4 shows there is a strong positive relationship between marital status,
age and income. While there is no direct relationship between age and income (Fig.
1), another scatterplot (Fig. 5) shows a clear correlation between income and total
sales per customer. Above average income demographic groups include:
 Widows ($56,957)
 USA ($53,525)
 PhD ($56,176)
This information will help to identify target groups for the upcoming advertising
campaign.
SQL was used to combine the advertising data (contained in a separate Excel
worksheet) with the sales data which allows us to easily examine any relationships
between advertising channel, product sales and demographics. Fig. 7 shows the
SQL statements. As a first step, a comparison between customer groups exposed to
a single advertising campaign would be interesting, using customers with no adverts
as the Control group. To achieve this, a new column String_ad was created to allow
for easy filtering (Fig. 8). Preliminary results showed (Fig. 8 & Fig. 9):
1. The Control group had an income lower than the average.
2. The Instagram group had the top sales.
3. Social media advertising campaigns targeted high income customers.
The data (removed outliers, duplicates and errors) was exported as CSV file and
imported into Tableau for further analysis and visualisation (Fig. 10).



Dashboard Design & Development

The dashboard design is based on solving the business problem and presenting this
information to the audience with an engaging narrative. In this case, the audience is
the Marketing Team, so a detailed knowledge of the business will be assumed.
Accessibility issues considered include:
 Good contrast between text and background
 Selection of colours with consideration to colour blind
people(blues/orange/grey)
 Explanatory headers, dimensions, tooltips and captions on charts
 Easy navigation
At the top of each dashboard page a summary of key statistics was provided for
easy reference, along with a brief explanation of the purpose of the page. Choice of
visualisation was determined by the data:
 Histograms were chosen to represent the distribution of age and income
 A map shows the count of customers by country
 Scatterplot to show relationships between two numerical variables (Income
vs. Average Sale)
 Bar charts were chosen to represent categorical data (Marital Status,
Education, Product) by a numerical value (Average Sales).
Interactivity was included on the dashboard to add more value to each section,
allowing the user to apply filters and show different sets of data by product and/or
demographic.
While the dashboard is specifically designed for the provided dataset, it can be
updated to inform decision-making from a live data feed.


Patterns, Trends & Insights

We want to know which advertising channel is most effective. The measure of
effectiveness will be the average sales. To measure effectiveness of different
advertising channels we can compare average sales between groups:
Control Group
(No Adverts)
Test Groups
(Brochure, Email, Twitter,
Facebook, Instagram)
The percentage difference between average sales of the control group and the test
groups will be compared. Fig. 9 illustrates the average income between the groups.
To ensure a fair comparison all customers with income lower than $60,000 were
filtered out, the results below are shown in Fig. 13.
1. Instagram was the most effective advertising channel, followed by Facebook.
2. Email was surprisingly effective at 21.8% increase compared to the control
group.
3. Twitter did not produce effective results.
Top selling products are alcohol, meat and commodities (see Fig. 14). Meat and fish
are of particular interest, as these items are perishable and have a high spoil rate,
and hence a higher profit.
Analysis (See Fig. 15, Fig. 16, Fig. 17) shows:
1. Combining Instagram with any other channel led to the most sales.
2. Impressive increases in our alcohol sales across all social media channels.
3. Sales in alcohol increased by 98.90% compared to the control group when
combining Instagram and Twitter.
4. Sales of meat and fish were best increased through Instagram and Facebook.
Product sales by demographic was analysed for customers with income above
$50,000:
Education (see Fig. 18)
 Masters group 9.95% higher average alcohol sales than Graduation
 PHD group 30.35% higher average alcohol sales than Graduation
Marital Status (see Fig. 19)
 Average sales of fish and meat highest in the Singles group
 High earning Singles may have more disposable income
Country (see Fig. 20)
 Alcohol sales strongest in Germany & Spain
 Sales of meat in India most impressive.



Key recommendations:


1. Collect all social media and email account data from customers.
2. Combine social media channels rather than using a single channel.
3. Advertising should be targeted at above average income groups.
4. Meat and fish sales increased using Instagram. Instagram can best be
combined with Facebook.
5. Use Instagram for alcohol promotions (must verify age > 18). Combine with
Twitter for good results.
6. Email is a cost-effective channel.

NOTE:
Please find the attached pdf report for detailed analysis.
