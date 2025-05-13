
---

## ✅ `README.md`

````markdown
# Bitcoin Sentiment vs Trader Performance Analysis

This project explores the relationship between Bitcoin market sentiment (Fear & Greed Index) and historical trading performance data. It merges and analyzes two datasets to extract insights that can drive smarter trading strategies.

---

## 📁 Datasets Used

1. **Fear and Greed Index Dataset**
   - Columns: `timestamp`, `value`, `classification`, `date`
   - Represents market sentiment on a given day.

2. **Hyperliquid Trader Data**
   - Columns include: `Account`, `Coin`, `Execution Price`, `Size Tokens`, `Size USD`, `Side`, `Timestamp IST`, `Start Position`, `Direction`, `Closed PnL`, etc.
   - Represents trade-by-trade history of accounts.

---

## 🧠 Objective

To analyze and understand how trader performance (profit/loss, trade direction, leverage, etc.) correlates with market sentiment (fear/greed). This includes:
- Comparing PnL on fear vs greed days
- Analyzing long/short strategies under different sentiments
- Studying leverage usage
- Identifying patterns across different traders

---

## ⚙️ Setup Instructions

1. Clone the repository or download the files.

2. Install dependencies:

```bash
pip install -r requirements.txt
````

3. Run the Python notebook or script provided in the repo to:

   * Clean and merge the data
   * Analyze performance trends
   * Visualize findings

---

## 📊 Features of the Analysis

* Average PnL per sentiment classification (Fear/Greed)
* PnL by trade direction (Long/Short)
* Correlation between sentiment value and PnL
* Visualization using Matplotlib and Seaborn
* Export of merged dataset as `merged_trader_sentiment.csv`

---

## 📝 Output

* CSV file with merged and cleaned data
* Box plots, bar charts, and scatter plots to visualize patterns
* Summary of insights and data-driven trading strategies

---

## 📈 Sample Insight

> Traders using long positions tend to make more profit on Greed days, while some contrarian traders perform well even during periods of Fear.

---

## 🔍 Folder Structure

```
project-folder/
│
├── fear_greed_index.csv
├── Historical_Data.csv
├── merged_trader_sentiment.csv
├── analysis_script.ipynb
├── requirements.txt
└── README.md
```

---

## 🙋 Author

Made as part of a data analysis assignment.

---

## ✅ License

This project is for academic and learning purposes only.

```
