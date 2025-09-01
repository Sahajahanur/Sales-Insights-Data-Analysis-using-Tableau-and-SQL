# Sales-Insights-Data-Analysis-using-Tableau-and-SQL
**********************************************************************************************************************************************************************************************************************************************
I am sharing India based Hardware company Sales Insights - A Data Analysis Project performed on Tableau & SQL in my journey into Data Science.
## About Project 👨‍💻
* Performed India based hardware company sales insights - A Data Analysis project.
* Developed ETL mappings using SQL to extract the data from unstructured data and transformed it to the staging area to conduct data cleaning and design star schema data model on Tableau.
* Developed a Tableau dashboard to perform analysis, producing quantitative visualizations in Tableau to draw valuable insights based on different parameters affecting the company performance year on year and further provide business solutions.
*********************************************************************************************************************************************************************************************************************************************
## Technologies used ⚙️
* Advance Excel excel
* MySQL mysql | SQL Server
* Tableau tableau | Power BI powerbi
* Statistics Statistics
*********************************************************************************************************************************************************************************************************************************************
## 📊 Tableau Dashboard  
[Profit Analysis Dashboard](https://public.tableau.com/app/profile/sahajahanur.laskar/viz/PROJECT1-Updated-Profit_Analysis/Dashboard-ProfitAnalysis?publish=yes)

### Problem Statements
Sales director wants to know the performance of the company in various Indian states & accordingly provide some discount.
* Q1. Revenue breakdown by cities.
* Q2. Revenue brekdown by years & months.
* Q3. Top 5 customers by revenue & sales quantity.
* Q4. Top 5 Products by revenue.
* Q5. Net Profit & Profit Margin by Market
### Approach - Project Planning & Aims Grid
1. Purpose: What? Why? What do we want to achieve?
To unlock sales insights that are not visible before for sales team for decision support & automate them to reduced manual time spent in data gathering.

2. Stake holders: Who will be involved?
  * Sales Director
  * I.T. Team
  * Customer Service Team
  * Data & Analytics Team.
3. End Result: What do we want to achieve?
An automated dashboard providing quick & latest sales insights to support data-driven decision making.
4. Success Criteria: What will be our success criteria?
* Dashboards uncovering sales order insights with latest data available.
*  Sales team able to take better decision & prove 10% cost savings of total spend.
*  Sales analysts stop data gathering manually to save 20% of their business time & reinvest it in value-added activity.
### Data Analysis - Approach

<img width="1365" height="822" alt="image" src="https://github.com/user-attachments/assets/b090cfa8-8e13-44ac-8972-a6135fed08a4" />

### Setup Process

**Step 1:** Download file : [db_dump.sql](https://github.com/Sahajahanur/Sales-Insights-Data-Analysis-using-Tableau-and-SQL/blob/main/database/db_dump.sql) or  [db_dump.xlsx](https://github.com/Sahajahanur/Sales-Insights-Data-Analysis-using-Tableau-and-SQL/blob/main/database/db_dump.xlsx)

Step 2: Import it in MySql do ETL(Extract, Transform, Load) if required

Step 3: Download [Tableau Public (Free)](https://www.tableau.com/products/public/download) or [Tableau Desktop (14 days trial)](https://www.tableau.com/products/desktop/download) to perform Data Analysis.

Step 4: Connect Tableau with MySql database or Excel database

Step 5: Save the file as (.twb or .twbx)

## Data Analysis Using SQL
1. Show all customer records

       SELECT * FROM customers;

2. Show total number of customers

       SELECT count(*) FROM customers;

3. Show transactions for Chennai market (market code for chennai is Mark001)

       SELECT * FROM transactions where market_code='Mark001';
4. Show distrinct product codes that were sold in Chennai.

       SELECT distinct product_code FROM transactions where market_code='Mark001';

5. Show transactions where currency is US dollars.

       SELECT * from transactions where currency="USD"
   
6. Show transactions in 2020 join by date table.

       SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;

7. Show total revenue in year 2020.

       SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";

8. Show total revenue in year 2020, January Month.

       SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");

9. Show the total revenue in the year 2020 in Chennai.

       SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020and transactions.market_code="Mark001";

## Data Analysis Using Tableau

### Creating Star Schema in Tableau

<img width="1623" height="817" alt="image" src="https://github.com/user-attachments/assets/0167611a-22dc-492c-8a93-9c8fa9dcac2a" />


### **Tableau Dashboard –** [Revenue Analysis](https://public.tableau.com/app/profile/sahajahanur.laskar/viz/PROJECT1-Updated/Dashboard-RevAnalysis?publish=yes)

<img width="1616" height="835" alt="image" src="https://github.com/user-attachments/assets/1ae21c68-5b50-42de-897f-b095572941ce" />

### **Tableau Dashboard –** [Profit Analysis](https://public.tableau.com/app/profile/sahajahanur.laskar/viz/PROJECT1-Updated-Profit_Analysis/Dashboard-ProfitAnalysis?publish=yes)

<img width="1571" height="832" alt="image" src="https://github.com/user-attachments/assets/be8afa7d-8b1a-4658-9f82-957c3a0e2745" />

### Project References: 🔗

## Project References: 🔗

| Sr.No. | References 👨‍💻 | Links 🔗 |
|--------|---------------|----------|
| 1 | **Tableau Project Dashboard :** Sales Insights - Data Analysis using Tableau | [Dashboard](https://public.tableau.com/app/profile/sahajahanur.laskar/viz/PROJECT1-Updated/Dashboard-RevAnalysis?publish=yes) |
| 2 | **Tutorial** | [YouTube Playlist](https://www.youtube.com/playlist?list=PLeo1K3hjS3utcb9nKtanhcn8jd2E0Hp9b) |
| 3 | **MySQL Installation** | [YouTube](https://www.youtube.com/watch?v=WuBcTJnIuzo) |
| 4 | **OLTP & OLAP** | [GeeksforGeeks](https://www.geeksforgeeks.org/dbms/difference-between-olap-and-oltp-in-dbms/) |
| 5 | **Star Schema: Fact Table & Dimension Table** | [Microsoft Docs](https://learn.microsoft.com/en-us/power-bi/guidance/star-schema) |

## For any queries/doubts 🔗 👇

## 📬 Contacts  

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:connectingsrl@gmail.com)  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sahajahanur-laskar/)









   



   



   



   






   










  




    










  





