# Product_review_project

## Project Purpose
The primary objective of this project is to enhance customer satisfaction by identifying key customer concerns and implementing internal measures for improvement. Throughout this project, tasks such as web data scraping, sentiment analysis, text labeling, and data visualization will be undertaken to gain valuable insights.

## Main Steps

![image](https://private-user-images.githubusercontent.com/92194263/324216966-4309584a-4554-4675-996d-a0c11bbc2a9f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzU4NzczNTYsIm5iZiI6MTczNTg3NzA1NiwicGF0aCI6Ii85MjE5NDI2My8zMjQyMTY5NjYtNDMwOTU4NGEtNDU1NC00Njc1LTk5NmQtYTBjMTFiYmMyYTlmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTAzVDA0MDQxNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTI4ODM5MGM5NmRhOGIwZDI2MjE1OTg4NjYxNDVkNzVhMjFiYTFhYTdmZWQyYWI0NGVkZDBhOTc1ODc4NGM2NGImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.1Uzku0UIMmJ9KOhxvfstKbzNvzt6cLd-cUrgxzp2Kgg)


### **1. Web scraping**

1.1 *Data Source*: 

[1] Company Website

- Fetch all the product name using python with selenium library, [check company product here](https://npicpet.com/collections/all)

[2] Amaozon

- First use instant data scraper to fetch existing data;

- After the pipeline built, use python to fetch the incoming new comments. 

*note: Since Amazon Anti-scraping technology keeps improving, the current code might not fit for future situation


### **2. Data Cleaning in Python**

- Fetch the comment datetime
- Transfer rate stars from text to float
- Select only product_id, username, rate_date, title, comment_body

### **3. OPENAI Labeling**

Appling OPENAI API to conduct labeling in three dimensions: 

1) Sentiment analysis: [Positive, Netural, Negative]
2) Complaint Category:
3) Quality Issues:

### **4. Database Build**

MySQL

- Design SQL schema
- Insert Cleaned data into database


### **5. Data Visualization**

Power BI

![image](https://github.com/Sol2023/product_review_project/assets/92194263/20c7e1a4-d5cb-4844-939a-c279f422fc9f)



## **To do**

- Keep fetching latest comment, automated the data pipeline.
- Modify the dashboard, make the trend of positive rate for each product when mouse float on it
- Add more marketing brand, and get insight with the market bench mark
