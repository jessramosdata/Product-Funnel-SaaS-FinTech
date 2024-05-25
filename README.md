# Product Funnel Analysis for SaaS FinTech

## Executive Summary:


### Business Problem: 

Completed orders are essential for this SaaS Fintech company since they're directly tied to revenue. Product and sales stakeholders have noticed that the product has a lower conversion rate than expected (based on users who start orders vs. complete the order). How can we determine where users are falling out of the workflow and make product adjustments to encourage users to complete their orders? 


### Methodology: 

1. SQL query that extracts, cleans, and transforms the data from the database
   
2. Build a dashboard in Power BI that tracks the number of orders in each status.

3. Conduct a more detailed funnel analysis in Python to simulate changes and determine the best areas of opportunity.


### Skills:

SQL: CTEs, Joins, Case, aggregate functions

Power BI: Dax, writing functions, ETL, calculated columns, data visualization, data modeling

Python: Pandas, Matplotlib, Numpy, Writing functions, building a product funnel, statistics






Summary: 

The Order Completion Flowchart visual (PDF located in the repository) shows the order completion metrics (described below) that were tracked to optimize order success. 

The Python model shows how to maximize order success and optimize revenue for our current product based on success rates for certain points in our software workflow. This helps identify where the opportunity is to create the biggest lift in revenue for the smallest lift in workflow completion metrics. It helps solve the business problem of identifying where customer workflow fallout needs to be improved. 

The function, **success**, models VOIE Order Completion metrics based on the given inputs. The input and output documentation is below. The function is designed to demonstrate how increases in the VOIE workflow metrics can affect VOIE KPIs and revenue.

## Function Inputs:

**inc_total_VOIE**: Amount to increase VOIE orders by (raw #)

**inc_interact_rate**: Amount to increase Interaction Rate by (%, should be between 0 & 1)

**inc_attempt_rate**: Amount to increase Login Attempt Rate by (%, should be between 0 & 1)

**inc_complete_rate**: Amount to increase Completed Login Rate by (%, should be between 0 & 1)

**labels**: Whether you want labels in your output (Binary variable, 1 provides labels & 0 doesn't)

## Function Outputs:

**VOIEs Started:** Total number of VOIE orders started.

**VOIEs Completed:** Total number of VOIE orders completed.

**Pullthrough:** The % of VOIE orders that are completed out of those that are interacted with.

**Borrower Conversion:** The % of VOIE orders that are completed out of the total VOIEs Started (includes those that are not interacted with).

**Revenue:** Total Revenue.


**NOTE:** The model is produced based on baseline metrics from the month of March 2022. Each change/increase put into the model will be based on the overall starting points from March.
