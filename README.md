# Product_review_project

## Project Purpose
The primary objective of this project is to enhance customer satisfaction by identifying key customer concerns and implementing internal measures for improvement. Throughout this project, tasks such as web data scraping, sentiment analysis, text labeling, and data visualization will be undertaken to gain valuable insights.

## Main Steps

![image](https://github.com/user-attachments/assets/6a819d6b-732e-4f34-aebc-fbdff177883f)



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

![image](https://github.com/user-attachments/assets/9dc85a1a-dcee-49aa-8aa8-f446924dfa50)




## **To do**

- Keep fetching latest comment, automated the data pipeline.
- Modify the dashboard, make the trend of positive rate for each product when mouse float on it
- Add more marketing brand, and get insight with the market bench mark
