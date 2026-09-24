# Telecom Customer Segmentation & Service Tier Analysis

**Author:** Aditya Pasarkar  
**Program:** AICTE | IBM SkillsBuild Data Analytics with AI Academic Internship  
**Partner Organization:** BharatCares  
**Primary Tech Stack:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)

---

## 📌 Executive Overview
This project delivers an end-to-end Data Analytics and Machine Learning solution to evaluate telecom customer demographics, income profiles, and tenure dynamics. By segmenting 1,000 active customer records into four service tiers, the project uncovers key drivers of service adoption and provides actionable business intelligence for customer retention and upselling.

### Key Performance Indicators (KPIs)
* **Total Customer Accounts Evaluated:** 1,000
* **Average Customer Income:** $77.53k
* **Average Customer Tenure:** 35.5 months
* **High-Value (Total Service) Share:** 23.60%

---

## 📁 Dataset & Schema Mapping
* **Dataset Name:** `teleCust1000t.csv`
* **Dimensions:** 1,000 rows × 13 features

| Feature Name | Type | Description |
| :--- | :--- | :--- |
| `region` | Categorical | Geographic region indicator |
| `tenure` | Continuous | Number of months the customer has stayed with the company |
| `age` | Continuous | Customer age in years |
| `marital` | Binary | Marital status (0 = Single, 1 = Married) |
| `address` | Continuous | Years lived at current address |
| `income` | Continuous | Household income in thousands ($k) |
| `ed` | Ordinal | Education level |
| `employ` | Continuous | Years with current employer |
| `retire` | Binary | Retirement status (0 = No, 1 = Yes) |
| `gender` | Binary | Gender indicator |
| `reside` | Continuous | Number of people residing in household |
| `custcat` | Target Variable | Customer Category ID (1 = Basic, 2 = E-Service, 3 = Plus, 4 = Total) |

---

## 📊 Business Intelligence & Key Findings

1. **Class Balance Across Tiers:**
   * **Plus Service:** 281 records (28.10%)
   * **Basic Service:** 266 records (26.60%)
   * **Total Service:** 236 records (23.60%)
   * **E-Service:** 217 records (21.70%)

2. **Core Upsell & Retention Drivers:**
   * **Tenure & Income:** Higher tenure (months with company) and household income show the strongest alignment with tier upgrades (Total Service and Plus Service).
   * **Feature Importance:** Random Forest classifier modeling confirms that `tenure`, `income`, `age`, and `address` (years at current residence) are the top predictive features driving customer service tier placement.

---

## 💡 Strategic Business Recommendations

* **Targeted Loyalty Programs:** Implement early-tenure incentives during the first 12–24 months to prevent early churn and accelerate progression toward higher tiers.
* **Middle-Tier Upselling:** Offer tailored bundled packages to middle-income households currently in the Basic or E-Service categories to transition them into Plus or Total Service.
* **VIP Retention Campaigns:** Dedicate proactive support resources to the **23.60% Total Service** account group to protect high-revenue streams.

---

## 📁 Repository Structure


├── teleCust1000t.csv                                # Raw Telecom Customer Dataset
├── AdityaPasarkar_TelecomCustomerSegmentation.ipynb # Complete Python EDA & Machine Learning Notebook
├── AdityaPasarkar_ProjectReport.docx               # Formal Project Report with Visualizations
├── README.md                                       # Project Documentation
└── requirements.txt                                # Python Package Dependencies
```

## ⚙️ Setup & Execution Instructions

1. **Clone the Repository:**
```bash
git clone https://github.com/YOUR_USERNAME/Telecom-Customer-Segmentation-IBM-SkillsBuild.git
cd Telecom-Customer-Segmentation-IBM-SkillsBuild
```

2. **Install Required Packages:**
```bash
pip install -r requirements.txt
```

3. **Run the Jupyter Notebook:**
```bash
jupyter notebook AdityaPasarkar_TelecomCustomerSegmentation.ipynb
```
