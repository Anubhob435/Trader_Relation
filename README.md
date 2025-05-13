
# 📊 Bitcoin Sentiment vs Trader Performance Analysis

![Bitcoin](https://img.shields.io/badge/Bitcoin-Analysis-orange)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-brightgreen)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

This comprehensive data analysis project investigates the relationship between Bitcoin market sentiment (using the Fear & Greed Index) and cryptocurrency trader performance metrics. By examining how traders behave and perform during different market sentiment conditions, we uncover patterns that can lead to more informed trading strategies and risk management approaches.

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [Datasets Used](#-datasets-used)
- [Key Research Questions](#-key-research-questions)
- [Installation & Setup](#-installation--setup)
- [Analysis Methodology](#-analysis-methodology)
- [Key Findings](#-key-findings)
- [Visualizations](#-visualizations)
- [Recommendations](#-recommendations)
- [Project Structure](#-project-structure)
- [Requirements](#-requirements)
- [How to Run](#-how-to-run)
- [Future Work](#-future-work)
- [License](#-license)

## 🔍 Project Overview

This analysis merges Bitcoin market sentiment data with detailed trader performance metrics from Hyperliquid to uncover hidden patterns in cryptocurrency trading behavior. The project addresses how market psychology (measured through the Fear & Greed Index) influences trading decisions, profitability, and risk-taking behavior.

Through statistical analysis and data visualization, we identify optimal trading strategies for different market sentiment conditions, patterns in trader behavior during sentiment shifts, and characteristics of consistently successful traders regardless of market sentiment.

## 📁 Datasets Used

### 1. Bitcoin Fear & Greed Index Dataset
- **Source**: Alternative.me API
- **Columns**: `timestamp`, `value`, `classification`, `date`
- **Description**: Daily sentiment measurements (0-100) categorized as Extreme Fear, Fear, Neutral, Greed, or Extreme Greed
- **Location**: `Data/fear_greed_index.csv`

### 2. Hyperliquid Trader Historical Data
- **Columns**: `Account`, `Coin`, `Execution Price`, `Size Tokens`, `Size USD`, `Side`, `Timestamp IST`, `Start Position`, `Direction`, `Closed PnL`, `Transaction Hash`, `Order ID`, `Crossed`, `Fee`, `Trade ID`, `Timestamp`
- **Description**: Detailed trade-by-trade history showing position entries, exits, sizes, and performance metrics
- **Location**: `Data/historical_data.csv`

## 🔎 Key Research Questions

1. How does market sentiment (Fear vs. Greed) impact trader performance (PnL)?
2. Which trading directions (Long/Short) perform better under different sentiment conditions?
3. How do traders adjust their behavior during shifts in market sentiment?
4. Can we identify traders who perform consistently across all sentiment conditions?
5. How does sentiment intensity (extreme fear to extreme greed) correlate with trading outcomes?
6. Are there measurable differences in trading volume, position size, or leverage during different sentiment periods?

## ⚙️ Installation & Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/bitcoin-sentiment-analysis.git
   cd bitcoin-sentiment-analysis
   ```

2. Set up a Python virtual environment (recommended):
   ```bash
   python -m venv venv
   # For Windows
   venv\Scripts\activate
   # For macOS/Linux
   source venv/bin/activate
   ```

3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

5. Open `bitcoin_sentiment_analysis.ipynb` to view and run the analysis

## 📊 Analysis Methodology

Our analytical approach combines:

1. **Data Preprocessing**:
   - Date format standardization and alignment
   - Merging datasets on date
   - Handling missing values
   - Feature engineering

2. **Exploratory Analysis**:
   - Distribution of PnL across sentiment categories
   - Trade volume and frequency by sentiment
   - Position size patterns

3. **Statistical Analysis**:
   - Correlation between sentiment values and trading metrics
   - Performance comparison across sentiment categories
   - Significance testing

4. **Advanced Analysis**:
   - Sentiment shift impact analysis
   - Trader consistency scoring
   - Strategy performance metrics
   - Time-series analysis

5. **Visualization**:
   - Distribution plots
   - Correlation charts
   - Time-series visualizations
   - Performance dashboards

## 🔑 Key Findings

1. **Sentiment-Performance Relationship**:
   - Traders achieved higher average PnL during Extreme Greed periods (67.89) compared to Extreme Fear periods (34.54)
   - Positive correlation exists between sentiment value and PnL

2. **Strategy Effectiveness**:
   - Long positions outperform during Greed conditions
   - Short positions show better performance during Fear conditions
   - Specific strategy combinations showed significantly higher win rates

3. **Trader Behavior**:
   - Distinct trading patterns emerge during sentiment shifts
   - Volume increases during extreme sentiment conditions
   - Position sizing varies systematically with sentiment

4. **Trader Consistency**:
   - Small subset of traders maintain consistent performance across sentiment conditions
   - These traders employ distinctly different strategies from the majority

5. **Sentiment Intensity Effects**:
   - Non-linear relationship between sentiment intensity and performance
   - Extreme sentiment levels show unique trading characteristics

## 📈 Visualizations

The notebook includes several visualization types:

1. **Distribution Analysis**:
   - Box plots of PnL by sentiment category
   - Histograms of trade sizes 

2. **Correlation Visualizations**:
   - Scatter plots of sentiment value vs. PnL
   - Heat maps of correlation matrices

3. **Time-Series Analysis**:
   - Line charts tracking sentiment changes over time
   - Performance metrics during sentiment shifts

4. **Strategy Comparison**:
   - Bar charts of strategy performance
   - Win rate and reward-risk visualizations

5. **Summary Dashboard**:
   - Combined visualization of key metrics and findings

## 🧠 Recommendations

Based on our analysis, we recommend:

1. **Sentiment-Based Strategy Adjustment**:
   - Favor short positions during Fear periods
   - Favor long positions during Greed periods
   - Adjust position sizing based on sentiment intensity

2. **Risk Management**:
   - Implement tighter stop-losses during extreme sentiment periods
   - Consider reducing leverage during sentiment transitions

3. **Performance Monitoring**:
   - Track strategy performance across different sentiment conditions
   - Develop metrics for evaluating sentiment-resilience

4. **Learning from Consistent Performers**:
   - Study trading patterns of consistently successful accounts
   - Adopt aspects of strategies that work across sentiment conditions

## 📂 Project Structure

```
bitcoin-sentiment-analysis/
│
├── Data/
│   ├── fear_greed_index.csv           # Bitcoin Fear & Greed Index data
│   └── historical_data.csv            # Hyperliquid trader performance data
│
├── Refined_data/
│   ├── merged_trader_sentiment.csv    # Merged dataset with basic analysis
│   └── complete_sentiment_analysis.csv # Enhanced dataset with all metrics
│
├── bitcoin_sentiment_analysis.ipynb   # Main analysis notebook
├── Bitcoin_Market_Sentiment_vs_Trader_Performance_Analysis.ipynb # Comprehensive version
├── requirements.txt                   # Python dependencies
├── DS Task.pdf                        # Project specification
└── README.md                          # This documentation
```

## 📝 Requirements

This project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

See `requirements.txt` for specific versions.

## 🚀 How to Run

1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Open `bitcoin_sentiment_analysis.ipynb` in the browser interface

3. Execute the cells in sequence to reproduce the analysis

4. Review the visualizations, findings, and recommendations

5. Optionally, export the notebook as HTML or PDF for sharing

## 🔮 Future Work

Potential extensions to this analysis include:

1. Incorporating additional sentiment indicators beyond the Fear & Greed Index
2. Developing predictive models to forecast trading performance based on sentiment
3. Analyzing sentiment impact with longer timeframes to identify seasonal patterns
4. Integrating market volatility metrics alongside sentiment data
5. Building an automated trading strategy that adapts to sentiment conditions

## ✅ License

This project is for academic and learning purposes only.

```
