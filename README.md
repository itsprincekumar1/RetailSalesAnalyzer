# 📊 Retail Sales Data Analyzer

A mini project using **PySpark** and **Pandas** to explore, clean, analyze, and visualize retail sales data!

---

## 🛠 Project Setup

- **Python Version**: 3.x
- **Libraries Used**:
  - `pyspark`
  - `findspark`
  - `matplotlib`
  - `seaborn`
  - `pandas`
  - `numpy`
- **Environment**:
  - Installed using **Anaconda Prompt**
  - Worked inside a virtual environment

---

## 📁 Project Structure

```
RetailSalesAnalyzer/
│
├── dataset/
│   └── OnlineRetailDataset.csv
│
├── outputs/
│   ├── data/
│   │   └── total_revenue_by_country.csv
│   │   └── cleaned_dataset.csv
│   └── plots/
│       └── total_revenue_by_country.png
│
│──retail_sales_analysis.ipynb
├── README.md
└── requirements.txt (optional)
```

---

## 📂 Data Source

- Dataset Name: **Retail Sales**
- Schema of the dataset:
  - Invoice: string (nullable = true)
  - StockCode: string (nullable = true)
  - Description: string (nullable = true)
  - Quantity: integer (nullable = true)
  - InvoiceDate: string (nullable = true)
  - Price: double (nullable = true)
  - Customer ID: integer (nullable = true)
  - Country: string (nullable = true)

---

## 🔎 Project Workflow

### 1. Data Ingestion
- Read CSV file using **PySpark**.

### 2. Data Cleaning
- Removed rows with:
  - Null values in important columns (`Invoice`, `StockCode`, `Price`, `Quantity`).
  - Negative or zero quantity and price.
- Corrected **InvoiceDate** into Timestamp format.

### 3. Data Exploration
- Checked schema using `printSchema()`.
- Summarized statistics using `describe()`.
- Counted unique invoices and customers.
- Verified countries involved in transactions.

### 4. Data Analysis
- **Total Revenue by Country**:
  - Grouped by "Country" and calculated total revenue (`Quantity * Price`).
- **Top-Selling Countries**:
  - Ordered countries by their total sales.
  
### 5. Data Visualization
- Created a **bar plot** showing total revenue by country using **Matplotlib** and **Seaborn**.

---

## 📈 Outputs

### ➡️ Data Outputs
- [`outputs/data/total_revenue_by_country.csv`](outputs/data/total_revenue_by_country.csv)
- [`outputs/data/cleaned_dataset.csv`](outputs/data/cleaned_dataset.csv)

### ➡️ Visual Outputs

| Total Revenue by Country |
|:-------------------------:|
| ![Total Revenue by Country](outputs/plots/total_revenue_by_country.png) |
| ![Total Products Sold](outputs/plots/Top_Products_Sold.png) |
| ![Sales Per Month](outputs/plots/Sales_per_Month.png) |

---

## 🚀 How to Run This Project

1. Clone this repository:

```bash
git clone https://github.com/your-username/RetailSalesAnalyzer.git
```

2. Install dependencies (optional):

```bash
pip install -r requirements.txt
```

3. Launch **Jupyter Notebook** inside your project folder:

```bash
jupyter notebook
```

4. Open `retail_sales_analysis.ipynb` and run all cells.

---

## ⚡ Future Enhancements

- Perform **monthly sales trend** analysis.
- Identify **top products** and **top customers**.
- Predict future sales using **machine learning models**.

---

## 🧠 Learnings

- Hands-on practice with **PySpark DataFrame API**.
- Real-world data cleaning challenges.
- Plotting and visualizing large datasets effectively.
- Project structure management for real deployment.

---

## 👨‍💻 Author

- **Name**: Prince
- **LinkedIn**: https://www.linkedin.com/in/prince5426/
- **GitHub**: https://github.com/itsprincekumar1

---

# 🚀 Let's Analyze Retail Like a Pro! 🔥

