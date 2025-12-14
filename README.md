Trader Behavior vs Market Sentiment Analysis
Overview

This project analyzes the relationship between market sentiment (Fear & Greed Index) and trader behavior using historical trading data from the Hyperliquid platform. The goal is to understand how profitability and trading activity vary across different sentiment regimes and to derive insights relevant to Web3 trading strategies.

Project Structure
ds_sandesh_naikwade/
│
├── notebook_1.ipynb        # Merging of Datasets
├── notebook_2.ipynb        # Main analysis notebook
│
├── csv_files/
│   ├── merged_data.csv
│
├── outputs/
│   ├── pnl_vs_sentiment.png
│   ├── tradecount_vs_sentiment.png
│   ├── pnl_distribution.png
│   └── profit_behavior_heatmap.png
│
├── ds_report.pdf           # Final summarized report
└── README.md

Datasets

Bitcoin Fear & Greed Index
Provides daily market sentiment classifications (Fear, Greed, etc.).

Historical Trader Data (Hyperliquid)
Contains trade-level records including timestamps, trade identifiers, and profit/loss values.

Raw datasets were sourced from the links provided in the assignment and processed into daily-level metrics for analysis.

Methodology

Cleaned and standardized both datasets

Aggregated high-frequency trade data to daily metrics

Merged trader behavior with market sentiment using date alignment

Performed exploratory data analysis to compare profitability and trading activity across sentiment regimes

Key Insights

Fear periods show higher and more consistent profitability, suggesting contrarian opportunities.

Greed periods exhibit higher trading activity but inconsistent returns, driven by a small number of extreme outcomes.

Market sentiment can be used as a contextual risk filter rather than a direct trading signal.

Limitations

Limited overlap between sentiment and trading datasets restricts sample size.

Leverage and account-level behavioral analysis were excluded due to limited availability of consistent identifiers in the aggregated daily dataset.

Findings should be interpreted as directional insights rather than statistically conclusive results.

Tools & Technologies

Python (Pandas, Matplotlib, Seaborn)

Jupyter / VS Code

CSV-based data processing

Author

Sandesh Naikwade

