E-commerce Data Analysis (Python)
This project performs sales data analysis from a CSV file (ecommerce.csv) using Python.
It includes:

data loading and validation,
descriptive statistics,
category-based revenue analysis,
monthly trend analysis,
a simple rule-based “AI chat” function for asking questions about the dataset.
🚀 Features
Data Loading

checks whether the file exists,
validates required columns.
Data Cleaning

converts Sales to numeric type,
removes missing critical values,
normalizes text fields (Category, Month),
keeps only valid month labels (Jan–Dec).
Preview and Statistics

head() for quick preview,
describe() for descriptive statistics.
Visualizations

bar chart: Revenue by Category,
line chart: Sales Trend Over Time (with proper month ordering).
Simple AI Chat (Rule-Based)

supported query types:
revenue
top category
top 3 category
average
unique customers
count
🛠 Requirements
Python 3.9+
libraries:
pandas
matplotlib
Install dependencies:

pip install pandas matplotlib
📁 Project Structure
Example structure:

.
├── analysis.py
├── ecommerce.csv
└── README.md
For Google Colab, the CSV file can be placed at: /content/ecommerce.csv

▶️ How to Run
Local environment
Put ecommerce.csv in the same directory as the script.
Set in code:
file_path = "ecommerce.csv"
Run:
python analysis.py
Google Colab
Upload ecommerce.csv to /content/
Set:
file_path = "/content/ecommerce.csv"
Run the notebook/script cells.
📄 Required CSV Format
Required columns:

Order_ID
Customer_ID
Category
Sales
Month
Example row:

Order_ID,Customer_ID,Category,Sales,Month
1,12,Home,60,Jan
💬 Example Questions for ask_ai
revenue
top category
top 3 category
average
unique customers
count
🧠 How ask_ai Works
The function uses keyword-based rules (if/elif) to detect intent and return results calculated from the pandas DataFrame.

It is not an LLM—it is a lightweight rule-based query assistant.

⚠️ Limitations
no advanced NLP,
limited number of supported intents,
no complex multi-condition filtering from natural language,
no direct BI/SQL integration in this script version (pandas + matplotlib only).
🔧 Possible Improvements
migrate to Streamlit for an interactive dashboard,
add SQLite and SQL querying,
extend NLP (e.g., top 5 in Jan, average in Feb),
export results to CSV/Excel,
integrate with Power BI / Looker Studio.
👨‍💻 Author
E-commerce data analysis project in Python.
Igor Michalak

## Business Questions

- Which category generated the most revenue?
- How did sales change over time?
- Which category should receive more attention?

## Key Findings

- Electronics generated the highest revenue.
- Revenue increased over time.

## Dashboard

<img width="872" height="501" alt="image" src="https://github.com/user-attachments/assets/5e0bbd3b-13cf-49c3-ad58-f3e3236209b4" />



## Trend Analysis

<img width="848" height="452" alt="image" src="https://github.com/user-attachments/assets/e58154f7-1d69-4458-bb89-1381549b7b4b" />

