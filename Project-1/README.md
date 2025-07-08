📊 Telecom Customer Churn Analysis

🌟 What’s This About?
This project looks at why customers leave a telecom company (called "churn"). We use a dataset to find patterns in customer info, like age, services, and bills, to help the company keep more customers. 😊

📂 The Data
The data comes from Kaggle: Telco Customer Churn. It has 7,043 rows and 38 columns, including:

👤 Customer Info: Age, Gender, Married or Not, Number of Dependents
📱 Services: Phone, Internet, Internet Type, Security, Streaming
💵 Billing: Monthly Bill, Total Bill, Total Money Spent, Payment Type, Contract
🚪 Churn Details: If they left (Churned), stayed (Stayed), or joined (Joined), and why they left


🎯 Goals

🔍 Check the Data: Look at the data to see what’s there and if anything’s missing.
📈 Find Patterns: See what makes customers leave, like their age or bills.
📊 Show Results: Use charts to make the findings clear and easy to understand.


🛠️ How We Did It
We used a Jupyter Notebook (Telecom-Churn-Analysis.ipynb) with Python. Here’s what we did:

🔎 Looked at the Data:

Checked the first few rows and data types.
Found missing info:
Churn Category and Churn Reason were empty for customers who didn’t leave.
Internet Type was missing for some customers without internet.




🧹 Cleaned the Data:

Filled empty Churn Category and Churn Reason with “Not Applicable” for customers who stayed.
Removed rows missing Internet Type to keep the data reliable.


📋 Analyzed the Data:

Calculated how long customers stay (tenure) based on whether they left or stayed.
Looked at how contract types (month-to-month, one-year, two-year) affect churn.
Key Findings:
Customers who stay have longer tenure (42.5 months) than those who leave (18.6 months).
Month-to-month contracts have a high churn rate (50.3%) compared to one-year (13.3%) or two-year (3.5%) contracts.




📉 Made Charts:

Age Chart (KDE Plot) 📊: Shows older customers (60+) are more likely to leave.
Correlation Heatmap 🔥: Shows Total Bills and Total Money Spent are closely related.
Contract Chart (Bar Plot) 📈: Shows month-to-month customers leave more often.
Bill Chart (Box Plot) 📉: Shows higher monthly bills might make customers leave.




🔑 What We Found

👴 Age: Customers over 60 are more likely to leave.
📜 Contracts: Month-to-month customers leave more than those with longer contracts.
💸 Bills: Higher monthly bills seem to lead to more churn.
⏳ Time with Company: Customers who stay longer are more loyal.


🧰 Tools Used

🐍 Python: The main programming language
📚 Pandas: For working with data
🔢 NumPy: For math and numbers
🎨 Matplotlib & Seaborn: For making charts
📓 Jupyter Notebook: For running the analysis


🚀 How to Run It

📋 What You Need:
Python 3.11.5
Install libraries: pip install pandas numpy matplotlib seaborn


📄 Steps:
Download the notebook (Telecom-Churn-Analysis.ipynb).
Put the dataset (telecom_customer_churn.csv) in the same folder.
Open Jupyter: jupyter notebook Telecom-Churn-Analysis.ipynb.
Run all cells to see the analysis and charts.




🔜 What’s Next?

🔍 Why They Leave: Look closer at reasons like “Competitor” or “Dissatisfaction.”
🤖 Predict Churn: Build a model to guess which customers might leave.
✨ New Features: Create new data points, like average bill per month.
🧑‍🤝‍🧑 Group Customers: Sort customers into groups for better retention plans.


📜 License
This project uses the MIT License.
