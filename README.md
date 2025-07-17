# Banking Analysis Dashboard

<img width="1161" height="640" alt="Screenshot 2025-07-17 140552" src="https://github.com/user-attachments/assets/542e1f76-ae5f-4097-be18-b5e15dbfd276" />
<img width="1163" height="652" alt="Screenshot 2025-07-17 140701" src="https://github.com/user-attachments/assets/32f5d5fd-9abb-42c3-ac0a-c1e510a90665" />
<img width="1163" height="647" alt="Screenshot 2025-07-17 140732" src="https://github.com/user-attachments/assets/14c49273-ae9e-41e5-b772-9e16a5b8427c" />
<img width="1160" height="647" alt="Screenshot 2025-07-17 140833" src="https://github.com/user-attachments/assets/f34cf1f5-c2e8-4bb2-b910-4d47ee37f091" />

<!-- Replace with actual screenshot -->

A comprehensive banking analysis solution that transforms raw client data into actionable insights through data cleaning, exploratory analysis, and interactive visualizations.

## Features

- **Data Processing Pipeline**: Automated cleaning and transformation of banking data
- **Exploratory Data Analysis**: In-depth analysis of client demographics and financial behavior
- **Interactive Dashboard**: Real-time visualization of key banking metrics
- **Client Segmentation**: Identification of high-value customers and risk profiles
- **Performance Tracking**: Monitoring of deposits, loans, and account engagement

## Technology Stack

### Data Processing
![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-blue?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-1.21+-blue?logo=numpy)

### Database
![MySQL](https://img.shields.io/badge/MySQL-8.0+-blue?logo=mysql)

### Visualization
![Power BI](https://img.shields.io/badge/Power_BI-Desktop-blue?logo=powerbi)

## Data Structure
The dataset contains comprehensive banking information with the following key attributes:

| Category | Key Metrics |
|----------|-------------|
| **Client Info** | Client ID, Name, Age, Gender, Nationality |
| **Accounts** | Checking Accounts, Saving Accounts, Foreign Currency Accounts |
| **Financials** | Bank Deposits, Credit Card Balance, Bank Loans, Superannuation Savings |
| **Relationship** | Loyalty Classification, Banking Contact, Joined Date |
| **Risk Analysis** | Risk Weighting, Properties Owned, Business Lending |

## Implementation Workflow

```mermaid
graph LR
A[Raw Data] --> B[Python Cleaning]
B --> C[MySQL Database]
C --> D[Exploratory Analysis]
D --> E[Power BI Dashboard]
E --> F[Business Insights]
```

## Dashboard Features
- **Client Demographics**: Age distribution, geographic analysis
- **Financial Health Metrics**: 
  ```dax
  // Sample DAX measure for engagement accounts
  Total Engagement = 
  SUM('Clients'[Checking Accounts]) + 
  SUM('Clients'[Saving Accounts]) +
  SUM('Clients'[Foreign Currency Account])
  ```
- **Revenue Analysis**: Fee structure performance by client segment
- **Risk Assessment**: Weighted risk scoring across portfolios
- **Relationship Insights**: Loyalty classification trends

## Getting Started

### Prerequisites
- Python 3.9+
- MySQL 8.0+
- Power BI Desktop

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/banking-analysis-dashboard.git
   ```
2. Set up the Python environment:
   ```bash
   pip install -r requirements.txt
   ```
3. Import database schema into your MySql Database from the csv file.

4. Run the ETL pipeline:
   ```bash
   python BankEDA_(Version_1).py
   ```
5. Open `dashboard.pbix` in Power BI Desktop

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Connect with me**: [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](your-linkedin-profile) 
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-green)](your-portfolio-link)

> "Without data, you're just another person with an opinion." - W. Edwards Deming
