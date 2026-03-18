# 💊 Quality Management Tool (CSV - Pharma)

## 🔗 Project Overview

The **Quality Management Tool** is a pharma-focused application built using **Python, CSV datasets, and validation principles** to simulate real-world **Computer System Validation (CSV)** in the pharmaceutical industry.

This project helps manage and analyze medicine-related data such as:

* Drug quality
* Batch records
* Manufacturing details
* Compliance checks
* Risk identification

The system follows **GxP guidelines** and demonstrates how data integrity and validation are maintained in regulated environments.

---

## 🎯 Objectives

* Ensure **data integrity and accuracy** in pharma datasets
* Implement **validation checks** as per CSV standards
* Analyze medicine data using Python
* Simulate **real-world quality management systems (QMS)**
* Detect anomalies, errors, and potential risks

---

## 🏗️ Tech Stack

* **Python** (Data Processing & Validation)
* **Pandas** (CSV handling & analysis)
* **NumPy** (Numerical operations)
* **Matplotlib / Seaborn** (Visualization - optional)
* **CSV Dataset** (Training & validation data)

---

## 📂 Project Structure

```
Quality-Management-CSV/
│
├── data/
│   ├── train_dataset.csv
│   └── test_dataset.csv
│
├── scripts/
│   ├── data_cleaning.py
│   ├── validation_checks.py
│   ├── analysis.py
│   └── report_generation.py
│
├── reports/
│   └── quality_report.pdf
│
├── README.md
└── requirements.txt
```

---

## 📊 Dataset Description

The dataset represents pharmaceutical product data with the following fields:

| Column Name        | Description                  |
| ------------------ | ---------------------------- |
| Medicine_Name      | Name of the drug             |
| Batch_ID           | Unique batch number          |
| Manufacturing_Date | Date of production           |
| Expiry_Date        | Expiry date                  |
| Temperature        | Storage temperature          |
| Humidity           | Storage humidity             |
| Quality_Status     | Pass/Fail                    |
| Defects            | Number of defects            |
| Compliance         | Regulatory compliance status |

---

## ⚙️ Features

### ✅ 1. Data Validation (CSV)

* Missing value detection
* Data type validation
* Range checks (Temperature, Humidity)
* Duplicate record detection

### ✅ 2. Quality Checks

* Batch failure detection
* Expired medicine identification
* Non-compliance detection

### ✅ 3. Risk Analysis

* High defect batches
* Storage condition violations
* Trend analysis of failures

### ✅ 4. Reporting

* Automated quality reports
* Summary dashboards
* CSV & PDF export

---

## 🔍 Sample Python Code

```python
import pandas as pd

# Load dataset
file_path = "data/train_dataset.csv"
df = pd.read_csv(file_path)

# Check missing values
print(df.isnull().sum())

# Identify failed batches
failed_batches = df[df['Quality_Status'] == 'Fail']
print(failed_batches)

# Check expired medicines
df['Expiry_Date'] = pd.to_datetime(df['Expiry_Date'])
expired = df[df['Expiry_Date'] < pd.Timestamp.today()]

print("Expired Medicines:")
print(expired)
```

---

## 🧪 CSV (Computer System Validation) Implementation

This project follows CSV lifecycle:

### 1. 📌 Planning Phase

* Define validation scope
* Risk-based approach

### 2. 📌 Requirement Phase

* User Requirement Specification (URS)

### 3. 📌 Testing Phase

* IQ (Installation Qualification)
* OQ (Operational Qualification)
* PQ (Performance Qualification)

### 4. 📌 Reporting Phase

* Validation report generation

---

## 📈 Use Cases

* Pharma companies for **quality monitoring**
* Regulatory audits and compliance checks
* Training project for **CSV + Python + Pharma domain**

---

## 🚀 How to Run

1. Clone the repository

```
git clone https://github.com/your-username/quality-management-csv.git
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Run scripts

```
python scripts/analysis.py
```

---

## 📌 Future Enhancements

* Integration with **SAP systems**
* Machine learning for defect prediction
* Real-time monitoring dashboard
* Cloud deployment

---

## 🤝 Contribution

Contributions are welcome! Feel free to fork and improve the project.

---

## 📄 License

This project is for educational purposes only.

---

## 👨‍💻 Author

**Sunil Singh Sisodia**

---

💡 *This project bridges Pharma Quality + CSV + Python to simulate real industry workflows.*
