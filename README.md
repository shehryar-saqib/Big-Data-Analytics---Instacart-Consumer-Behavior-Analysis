# Instacart Consumer Behavior Analysis

This repository offers a complete workflow for understanding and predicting shopper behaviors on Instacart’s 2017 dataset.

## ⚙️ What You’ll Find

* **Data Preparation:** Clean, validate, and enhance raw CSVs for reliable analysis.
* **Exploratory Data Analysis:** Interactive charts to spot trends in ordering patterns.
* **Customer Segmentation:** RFM (Recency, Frequency, Monetary) analysis and clustering to group similar shoppers.
* **Predictive Modeling:** Train and evaluate models that forecast customers’ next product purchases.
* **Market Basket Analysis:** Discover association rules that reveal common item combinations.

## 📁 Project Layout

```plaintext
project-root/
├── data/               # Raw and processed data
│   ├── original/       # Downloaded Instacart CSVs
│   └── processed/      # Cleaned datasets for analysis
├── notebooks/          # Jupyter notebooks showcasing analyses
├── src/                # Reusable Python modules and scripts
├── models/             # Serialized machine learning models
├── requirements.txt    # Project dependencies
└── README.md           # This guide
```

## 🚀 Getting Started

1. **Clone the repo:**

   ```bash
   git clone <repo_url>
   cd project-root
   ```
2. **Set up a virtual environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate    # Windows
   ```
3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```
4. **Prepare the data:**

   ```bash
   python src/preprocessing.py --input data/original --output data/processed
   ```
5. **Explore with notebooks:**

   ```bash
   jupyter lab notebooks/
   ```
6. **Train models & evaluate:**

   ```bash
   python src/modeling.py --data data/processed --output_dir models
   ```

## 📈 Key Takeaways

* **RFM Insights:** Identified core customer segments based on purchase behavior.
* **Association Rules:** Uncovered popular product pairings for cross-selling opportunities.
* **Model Performance:** Achieved approximately 75% accuracy in next-item predictions.
