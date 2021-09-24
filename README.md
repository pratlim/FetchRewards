# FetchRewards
### Challenge 1: Diagram a New Structured Relational Data Model

The Relational Data Model consisted of four tables such as Users, Brands, Receipts and RewardsReceiptsItemList. 

### Challenge 2: Queries for the questions from business stakeholders
The queries/answers to the questions are in the file with the title “SQL_Queries.pdf”

### Challenge 3: Data Quality Issues in the Data
The data quality issues and solutions to overcome these issues are discussed in the Jupyter Notebook with the title “FetchRewards.ipynb”
Here, the data is converted from JSON to CSV format for the easier execution of data analysis part and for the data analysis and exploration purpose, Python programming language is used. 
Some of the data quality issues faced during the exploration of the files (Users, Brands, Receipts):
1.	Null/NA Values present
2.	Duplicate records – there are multiple instances where duplicate IDs with respective attributes are duplicated 
3.	Wrong formatting of the data – Date is stored in the 13-digit number instead of standard format of timestamp, Title names are written in the wrong format
Through data cleaning and formatting processes, data quality issues from the data have been removed. For these processes, several python functions, and libraries (Pandas, NumPy) are used. 
Also, many records from rewardsReceiptItemList possess barcode as ‘4011’ which is nothing but ‘Item not found’ case. As cost of these products are getting added to the Total Spent, it is not correct to remove these products directly during data cleaning process. 
Addition to this, this column has many items barcodes whose values are not matching with the barcodes from the Brands table. So, it is difficult to track them down. Therefore, the join between the tables Brands and RewardsReceiptsItemList is with brand name -> description and not with the barcode. 

### Challenge 4: Communicate with stakeholders
The email to business people/ Stakeholders is in the file with the title ""
