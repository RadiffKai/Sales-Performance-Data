# Sales-Performance-Data
An interactive Excel analytics solution designed to evaluate, sales performance, profitability, customer segment, order fulfillment, regional performance, product performance.  

<img width="930" height="424" alt="Screenshot 2026-10-03 185423" src="https://github.com/user-attachments/assets/93f007c0-fa53-402d-a0dc-b74f9ea00618" />  

## Tools
1. Microsost Excel Power Query
2. Power Pivot
3. Pivot tables, slicers and timelines
   
### Project overview
This project analyses a superstore-style retail dataset  containing each order row(order date,ship date, quantity, price,discount etc)
Final output is a one page interactive management dashboard that allow users  to investigate sales profitability, customer segment etc  
 Below are the some of question i had to answer before making the dashboard.  
 <img width="625" height="419" alt="Screenshot 2026-10-04 131251" src="https://github.com/user-attachments/assets/bf8ab548-1cbe-443d-b25f-6693760aa1ce" />
## Data  
Key fields: OrderID, Order Date, Ship Date, Ship Mode, Customer ID, Customer Name, Segment, Region, State, City, Category, Sub-Category, Product, Sales, Quantity, Discount, Profit  
The dataset covers multiple years of retail transaction and multiple dimensions to analyze  
## Analytical Workflow  
The project followed ETL-to-insight workflow:  
Profiling the data ; no of rows, what one row represents, data type, data ranges  
Data quality Audit ; missing values, incorrect data type, invalid date, inconsitent ranges  
Data transformation; i used power query to transform the data, one important issue occurred with date fields where i had to use change locale to correctly interpret US-formatted dates.  
<img width="899" height="464" alt="Screenshot 2026-10-04 143009" src="https://github.com/user-attachments/assets/903e5a7e-d97d-4d0e-a8db-cb734ad01b83" />

Some business validation such as making sure that  ship date >= order date, then got the shipping days which aided in understanding fulflment performance.  
Loaded the data to power pivot  into a model; where measures,relationship,kpi calculaion, distinct order calculation, reusable DAX logic plus creating a date table.  

<img width="629" height="393" alt="Screenshot 2026-10-04 142726" src="https://github.com/user-attachments/assets/40b6ee4d-e4b6-42dd-b469-81ccf37fc3fb" />  

Final dashboard was designed as a single-page management interface interactive filters, main visual analysis include (sales and profit trends, sales by category, profit by region, top subcategory by profit ,operational shipping performance among others)  

 ### Limitation   
 1. The data doesn't represent the real world commercial database
 2. Historical observation could not by itself establish causal relationship
    
### Future development    
Developing predictive demand - discount model  

### Skills demonstrated  
1. Data profilling
2. Data Quality Assesment
3. ETL
4. Exploratory analysis
   
### Conclusion  
The primary objective was to demonstrate that excel can be used not merely as a spreadsheet tool ,but as an analytical environment for : cleaning data,  modelling data, measuring performance, investigating business problem, and communicate decisions.


