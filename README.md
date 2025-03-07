# Marketing Analytics & Regression (MSIN0094)

This repository contains assignments and analyses for the **MSIN0094** course, focusing on **Marketing Analytics, Regression Modeling, and Machine Learning Techniques** for business decision-making. The projects involve data wrangling, regression analysis, clustering, decision trees, and A/B testing.

---

## 📂 Repository Structure

```
📁 MSIN0094-Marketing-Analytics
│── 📄 README.md                 # Overview of the project
│── 📂 data                      # Datasets used in analysis
│── 📂 code                      # R scripts and QMD files for analysis
│── 📂 reports                   # PDFs and markdown reports of assignments
│── 📂 results                   # Outputs from models and visualizations
```

---

## 📊 Project Components

### 1️⃣ **Data Wrangling & Merging**
- **Objective:** Clean and merge multiple datasets (sales, product, and marketing).
- **Techniques Used:** `left_join()`, `right_join()`, `dplyr`, and `mutate()` in R.
- **Key Output:** `data_full` dataset combining all relevant data.

### 2️⃣ **Marketing Mix Modeling (Regression Analysis)**
- **Objective:** Analyze the impact of marketing spend and pricing on sales.
- **Techniques Used:** Linear regression using `fixest::feols()`.
- **Key Findings:**
  - A $1 increase in final price results in **0.002** additional sales.
  - A $1 increase in marketing expense increases sales by **0.049** units.

### 3️⃣ **Customer Segmentation (K-Means Clustering)**
- **Objective:** Identify high-response customer segments.
- **Techniques Used:** `kmeans()` clustering on Recency, Frequency, and Monetary Value (RFM).
- **Findings:** 
  - **Segment 2** had the highest response rate (12.6%).
  - Targeting this segment resulted in a **25.6% ROI**.

### 4️⃣ **Decision Trees & Random Forest**
- **Objective:** Predict customer subscription likelihood.
- **Techniques Used:** `rpart` for Decision Trees and `ranger` for Random Forest.
- **Findings:**
  - **Decision Tree ROI:** **71.9%**
  - **Random Forest ROI:** **42.9%**
  - **Tradeoff:** Decision Trees are interpretable, while Random Forest is more robust.

### 5️⃣ **A/B/N Testing for Marketing Campaigns**
- **Objective:** Evaluate marketing effectiveness using controlled experiments.
- **Methodology:**
  - Divided customers into groups using **Decision Trees, Random Forest, K-Means, and a Control Group**.
  - Tested conversion rates and ROI for each method.
- **Findings:** Decision Trees provided the **best ROI and targeting efficiency**.

---

## 🔧 Installation & Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/MSIN0094-Marketing-Analytics.git
   cd MSIN0094-Marketing-Analytics
   ```
2. Install dependencies in R:
   ```r
   install.packages(c("tidyverse", "fixest", "broom", "rpart", "rpart.plot", "ranger", "factoextra"))
   ```
3. Run the R scripts (`.qmd` and `.R` files) using RStudio or Quarto.

---

## 📜 License

This project is for **educational purposes** only. Please do not distribute without permission.

---

## 📩 Contact

For questions, reach out via GitHub issues or email: `your-email@example.com`.
