# KingCounty_Housing

## 🎯 Project goal
Create a dashboard for house sales transactions for buyers/investors. Visualise key information like transaction price and include the relationship between view and condition. 

## 🛠️ Tools
- Microsoft Excel for data cleaning
- Tableau for data visualisation - View [dashboard](https://public.tableau.com/app/profile/harry.bui/viz/KingCountryHouseSales2014-2015/KingCountyHouseSales?publish=yes)

## 🪥 Data cleaning
### Convert the CSV file to Excel

- A preview of the data:
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/de799415-119f-4a6d-8286-944a70be44f4)

### Ensure the correct data type for each column
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/9fe22e95-971f-4230-bc0c-76336dfe7368)

### Check for duplicates
- Row count = 21613
- Unique id = 21436
Are there duplicates that we need to remove?
Upon further inspection, there are 176 ids that seems to be duplicated in 353 transactions, but these are houses that were transacted 2 or 3 times within the period. 
Conclusion: no duplicates that need to be removed.

### Remove 0 bedroom or 0 bathroom houses
- It seems inaccurate that a house has 0 bedroom or 0 bathroom so these records were removed.
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/13c96c6d-b5d2-40e2-91e9-3dc76d033928)

- Similarly, houses with 0 bathroom are probably uninhabitable so these records were removed.
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/4a9f1df9-2ecb-44dd-a18e-4b0541557dfd)
There are properties with 0 bedroom but come with bathrooms, they can be self contained studios so those records were not removed.

### Convert sqft to sqm
1 square foot = 0.09290304 square metre
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/5360a5c6-9197-4c25-b346-d173f672a322)

### Convert the characteristic columns from number to categorical string
Specifically these columns: waterfront, view, condition
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/afa9f30c-cc3f-4327-b825-9cdb834c743a)

## 📊 Load Data into Tableau
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/0cd7b353-1b69-4e45-a5b9-e2f7ab773b2c)

## 🖼️ Dashboard
![image](https://github.com/HarryQBui/KingCounty_Housing/assets/95842183/b8c09bb4-be13-42dd-820a-b6174c8fab2f)


