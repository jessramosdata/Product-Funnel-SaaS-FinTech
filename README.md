# Product Funnel Analysis for SaaS FinTech

## Executive Summary:

Using SQL, Python, and Power BI, I pulled order status data from the database and created a dashboard to track orders through the funnel. After identifying that the largest revenue opportunities are to increase user interaction rate and completed login attempts, I recommend that the product team implements a few adjustments that will lead to higher conversion:

1. Copy changes within the workflow
2. Reminder emails/texts
3. Better client relationships


### Business Problem: 

Completed orders are essential for this SaaS Fintech company since they're directly tied to revenue. Product and sales stakeholders have noticed that the product has a lower conversion rate than expected (based on users who start orders vs. complete the order). How can we determine where users are falling out of the workflow and make product adjustments to encourage users to complete their orders? 

![Screenshot 2024-05-25 at 2 05 24 PM](https://github.com/jessramosdata/Product-Funnel-SaaS-FinTech/assets/59672972/be7317e4-175b-4442-8091-8c4fb99854ac)



### Methodology: 

1. SQL query that extracts, cleans, and transforms the data from the database.
   
2. Build a dashboard in Power BI that tracks the number of orders in each status.

3. Conduct a more detailed funnel analysis in Python to simulate changes and determine the best areas of opportunity.


### Skills:

SQL: CTEs, Joins, Case, aggregate functions

Power BI: Dax, writing functions, ETL, calculated columns, data visualization, data modeling

Python: Pandas, Matplotlib, Numpy, Writing functions, building a product funnel, statistics


### Results & Business Recommendation: 

Creating a dashboard to track product orders gives product and sales stakeholders visibility into the product funnel both overall and for specific clients. Because of democratizing this data, stakeholders are now able to self serve, and the analytics team now has 5 less hours of ad hoc requets per week. This analysis showed us that almost 50% of orders fall out before entering the workflow, and less than 25% of users enter their correct banking credentials to connect their account. According to the model built in Python, increasing user interaction rates by 1% will result in $285 more in daily revenue and increasing completed bank login attempts by 1% will result in $405 more in daily revenue.

![Screenshot 2024-05-25 at 2 04 48 PM](https://github.com/jessramosdata/Product-Funnel-SaaS-FinTech/assets/59672972/d8cbde85-be7e-4c16-a132-02a63e357b1d)


Because the biggest revenue impacts will likely come from increasing the user interaction rate & completed login attempts, I recommend a few product adjustments: 

1. Send inactive users reminder emails and texts to encourage them to enter the platform to complete their order.
2. Work with clients (mortgage lenders) to help coach the users through the process and see the value in doing so.
3. Add copy at the beginning of the workflow stating that the process only takes 5 min, and feature a progress bar throughout.
4. Add copy at the bank login page to encourage users to look up their credentials to make sure they're correct.

I believe these adjustments will best tackle the largest workflow fallout points, increase conversion & revenue, and save the analytics team hours per week from a decrease in ad hoc requests.

### Next Steps: 

1. AB Test copy within the workflow
2. Train clients and users
3. Measure email and text open & click rates


