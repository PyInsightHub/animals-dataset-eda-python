# 🐾 Animals Dataset EDA (Python)

Exploratory data analysis of an animal taxonomy dataset, covering data cleaning, statistical analysis, visualization and key findings.

## 📌 Project Overview

This project analyzes 1,349 animal records described by their biological classification, from Kingdom down to Genus. The goal is to understand the composition of the dataset, assess its data quality, and present the findings clearly.

## 📂 Repository Structure

```
animals-dataset-eda-python/
├── animals.csv                  # Source dataset
├── Animals.ipynb                # Analysis notebook
├── Animal_Data_Summary.pptx     # Summary presentation
└── README.md
```

## 📊 Dataset Description

| Attribute | Detail |
|---|---|
| Records | 1,349 |
| Columns | 19 (18 descriptive fields plus an exported row index) |
| Unique animal names | 1,226 |
| Classes | 3 (Mammalia, Aves, Reptilia) |
| Orders | 55 |
| Families | 210 |

Fields include Animal Name, Kingdom, Phylum, Subphylum, Class, Order, Suborder, Family, Subfamily, Genus and other taxonomic ranks.

## 🔄 Analysis Workflow

1. **Import** the libraries and load the data
2. **Data inspection**: shape, data types, summary statistics, missing values and duplicates
3. **Exploratory data analysis**: class, family and order breakdowns
4. **Statistical analysis**: frequency, percentage and cross-tabulation analysis
5. **Visualization**: bar charts, pie charts and count plots
6. **Insights**: summary of key findings

## 🔍 Key Findings

- **Mammalia** dominates the dataset with 815 records (60.4%), followed by **Aves** (328, 24.3%) and **Reptilia** (206, 15.3%).
- **Bovidae** is the largest family (69 records, 5.1%). The top 10 families account for 31.2% of all records.
- Core fields (Name, Class, Order, Family) are **100% complete**, while finer ranks such as Subclass (4.6%) and Subgenus (1.3%) are sparse. Some ranks may simply not apply to certain animals.
- 123 animal names appear more than once, so a targeted data-quality check is recommended before further modeling.
- The class imbalance should be taken into account in any comparison or predictive modeling.

> Note: These findings describe the records in this dataset, not global animal diversity or population abundance.

## 🛠 Tools & Technologies

- Python
- Pandas, NumPy
- Matplotlib, Seaborn, Plotly
- Jupyter Notebook / Google Colab

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/animals-dataset-eda-python.git
   cd animals-dataset-eda-python
   ```
2. Install the dependencies
   ```bash
   pip install pandas numpy matplotlib seaborn plotly jupyter
   ```
3. Open the notebook
   ```bash
   jupyter notebook Animals.ipynb
   ```
4. Make sure the file path in the notebook points to `animals.csv`. The original notebook uses `/content/animals.csv` for Google Colab.
