# Trading Data Analysis Project

This project analyzes trading performance data in correlation with market sentiment to identify patterns and insights for trading strategy optimization.

---

## Overview

This analysis combines trader transaction data with market sentiment classifications to explore:

* **Trading behavior patterns** across different market sentiments
* **Profitability analysis** by market conditions
* **Trade volume distribution** across sentiment categories
* **Daily trading trends** and performance metrics

---

## Features

* **Data Integration**: Merges trader data with sentiment analysis data.
* **Comprehensive Visualizations**: Generates multiple charts and plots for in-depth analysis.
* **Performance Analytics**: Analyzes PnL (Profit and Loss) across various market conditions.
* **Trend Analysis**: Identifies daily trading patterns and sentiment correlations.
* **Automated Setup**: Creates an organized directory structure for all outputs.

---

## Prerequisites

* Python 3.7+
* Google Colab environment (recommended)
* Internet connection for downloading datasets

---

## Required Libraries

The project relies on the following Python libraries:

* `pandas`
* `matplotlib`
* `seaborn`
* `gdown`

---

## Installation

1.  Clone or download the project files.
2.  Run the script in Google Colab or Jupyter Notebook.
    The script will automatically install required dependencies:
    ```bash
    pip install -q pandas matplotlib seaborn gdown
    ```

---

## Data Sources

The project uses two datasets hosted on Google Drive:

### Trader Data (`trader_data.csv`)

Contains trading records with timestamps, trade sides, sizes, and PnL.
**Fields include**: `Timestamp IST`, `Side`, `Size USD`, `Closed PnL`

### Sentiment Data (`sentiment_data.csv`)

Contains daily market sentiment classifications.
**Fields include**: `date`, `classification`

---

## Project Structure

After running the script, the following directory structure is created:

ds_Gaurav_Adhikari/
├── csv_files/
│   ├── trader_data.csv
│   ├── sentiment_data.csv
│   └── merged_data.csv
└── outputs/
├── trades_by_sentiment.png
├── profitability_vs_sentiment.png
├── volume_vs_sentiment.png
├── daily_trade_count_trend.png
└── daily_avg_pnl_trend.png


---

## Usage

1.  Run the complete script in Google Colab or Jupyter Notebook.
2.  **Data Download**: The script automatically downloads datasets from Google Drive.
3.  **Data Processing**: Cleans and preprocesses the data, handling missing values.
4.  **Analysis Generation**: Creates visualizations and saves them to the `outputs` folder.
5.  **Review Results**: Check the generated plots and the `merged_data.csv` dataset.

---

## Generated Visualizations

The script generates the following key visualizations:

1.  **Trades by Market Sentiment and Side**
    * **File**: `trades_by_sentiment.png`
    * **Description**: Count plot showing trade distribution across sentiment categories and trade sides (buy/sell).

2.  **Profitability vs Market Sentiment**
    * **File**: `profitability_vs_sentiment.png`
    * **Description**: Box plot analyzing PnL distribution across different market sentiments.

3.  **Trade Volume vs Market Sentiment**
    * **File**: `volume_vs_sentiment.png`
    * **Description**: Violin plot showing trade size distribution by market sentiment.

4.  **Daily Trade Count Trend**
    * **File**: `daily_trade_count_trend.png`
    * **Description**: Line plot tracking daily trading activity by sentiment over time.

5.  **Daily Average PnL Trend**
    * **File**: `daily_avg_pnl_trend.png`
    * **Description**: Line plot showing daily average profitability trends by sentiment.

---

## Key Analysis Points

* **Sentiment Impact**: Identifies how market sentiment affects trading behavior.
* **Risk Assessment**: Analyzes profitability patterns across different market conditions.
* **Volume Analysis**: Examines trade size variations with sentiment changes.
* **Temporal Patterns**: Tracks daily trading and profitability trends.

---

## Data Processing Steps

The project follows these data processing steps:

* **Data Loading**: Downloads and loads CSV files into pandas DataFrames.
* **Datetime Conversion**: Converts timestamp columns to proper datetime format.
* **Data Cleaning**: Removes rows with missing values to ensure data quality.
* **Data Merging**: Combines trader and sentiment data on date keys for integrated analysis.
* **Aggregation**: Creates pivot tables for comprehensive trend analysis.

---

## Output Files

* **Merged Dataset**: `merged_data.csv` - The combined trader and sentiment data.
* **Visualizations**: PNG files saved in the `outputs/` folder.
* **Console Output**: Data previews and processing status messages.

---

## Customization

To modify or extend the analysis:

* **Change Data Sources**: Update the Google Drive URLs in the script.
* **Modify Visualizations**: Adjust `matplotlib`/`seaborn` parameters for different chart styles or aesthetics.
* **Add Analysis**: Extend the script with additional metrics or visualizations.
* **Filter Data**: Add date ranges or other filtering criteria to focus your analysis.

---

## Troubleshooting

* **Download Issues**: Ensure Google Drive links are accessible and properly formatted.
* **Missing Data**: The script handles missing values by dropping affected rows.
* **Plot Display**: In some environments, use `plt.show()` to display plots.
* **Memory Issues**: For large datasets, consider processing data in chunks.

---

## Dependencies

* `pandas`: For data manipulation and analysis.
* `matplotlib`: For basic plotting functionality.
* `seaborn`: For statistical data visualization.
* `gdown`: For downloading Google Drive files.
* `os`: For directory and file operations.

---

## Author

Gaurav Adhikari

# Trading Data Analysis Project

This project analyzes trading performance data in correlation with market sentiment to identify patterns and insights for trading strategy optimization.

---

## Overview

This analysis combines trader transaction data with market sentiment classifications to explore:

* **Trading behavior patterns** across different market sentiments
* **Profitability analysis** by market conditions
* **Trade volume distribution** across sentiment categories
* **Daily trading trends** and performance metrics

---

## Features

* **Data Integration**: Merges trader data with sentiment analysis data.
* **Comprehensive Visualizations**: Generates multiple charts and plots for in-depth analysis.
* **Performance Analytics**: Analyzes PnL (Profit and Loss) across various market conditions.
* **Trend Analysis**: Identifies daily trading patterns and sentiment correlations.
* **Automated Setup**: Creates an organized directory structure for all outputs.

---

## Prerequisites

* Python 3.7+
* Google Colab environment (recommended)
* Internet connection for downloading datasets

---

## Required Libraries

The project relies on the following Python libraries:

* `pandas`
* `matplotlib`
* `seaborn`
* `gdown`

---

## Installation

1.  Clone or download the project files.
2.  Run the script in Google Colab or Jupyter Notebook.
    The script will automatically install required dependencies:
    ```bash
    pip install -q pandas matplotlib seaborn gdown
    ```

---

## Data Sources

The project uses two datasets hosted on Google Drive:

### Trader Data (`trader_data.csv`)

Contains trading records with timestamps, trade sides, sizes, and PnL.
**Fields include**: `Timestamp IST`, `Side`, `Size USD`, `Closed PnL`

### Sentiment Data (`sentiment_data.csv`)

Contains daily market sentiment classifications.
**Fields include**: `date`, `classification`

---

## Project Structure

After running the script, the following directory structure is created:

ds_Gaurav_Adhikari/
├── csv_files/
│   ├── trader_data.csv
│   ├── sentiment_data.csv
│   └── merged_data.csv
└── outputs/
├── trades_by_sentiment.png
├── profitability_vs_sentiment.png
├── volume_vs_sentiment.png
├── daily_trade_count_trend.png
└── daily_avg_pnl_trend.png


---

## Usage

1.  Run the complete script in Google Colab or Jupyter Notebook.
2.  **Data Download**: The script automatically downloads datasets from Google Drive.
3.  **Data Processing**: Cleans and preprocesses the data, handling missing values.
4.  **Analysis Generation**: Creates visualizations and saves them to the `outputs` folder.
5.  **Review Results**: Check the generated plots and the `merged_data.csv` dataset.

---

## Generated Visualizations

The script generates the following key visualizations:

1.  **Trades by Market Sentiment and Side**
    * **File**: `trades_by_sentiment.png`
    * **Description**: Count plot showing trade distribution across sentiment categories and trade sides (buy/sell).

2.  **Profitability vs Market Sentiment**
    * **File**: `profitability_vs_sentiment.png`
    * **Description**: Box plot analyzing PnL distribution across different market sentiments.

3.  **Trade Volume vs Market Sentiment**
    * **File**: `volume_vs_sentiment.png`
    * **Description**: Violin plot showing trade size distribution by market sentiment.

4.  **Daily Trade Count Trend**
    * **File**: `daily_trade_count_trend.png`
    * **Description**: Line plot tracking daily trading activity by sentiment over time.

5.  **Daily Average PnL Trend**
    * **File**: `daily_avg_pnl_trend.png`
    * **Description**: Line plot showing daily average profitability trends by sentiment.

---

## Key Analysis Points

* **Sentiment Impact**: Identifies how market sentiment affects trading behavior.
* **Risk Assessment**: Analyzes profitability patterns across different market conditions.
* **Volume Analysis**: Examines trade size variations with sentiment changes.
* **Temporal Patterns**: Tracks daily trading and profitability trends.

---

## Data Processing Steps

The project follows these data processing steps:

* **Data Loading**: Downloads and loads CSV files into pandas DataFrames.
* **Datetime Conversion**: Converts timestamp columns to proper datetime format.
* **Data Cleaning**: Removes rows with missing values to ensure data quality.
* **Data Merging**: Combines trader and sentiment data on date keys for integrated analysis.
* **Aggregation**: Creates pivot tables for comprehensive trend analysis.

---

## Output Files

* **Merged Dataset**: `merged_data.csv` - The combined trader and sentiment data.
* **Visualizations**: PNG files saved in the `outputs/` folder.
* **Console Output**: Data previews and processing status messages.

---

## Customization

To modify or extend the analysis:

* **Change Data Sources**: Update the Google Drive URLs in the script.
* **Modify Visualizations**: Adjust `matplotlib`/`seaborn` parameters for different chart styles or aesthetics.
* **Add Analysis**: Extend the script with additional metrics or visualizations.
* **Filter Data**: Add date ranges or other filtering criteria to focus your analysis.

---

## Troubleshooting

* **Download Issues**: Ensure Google Drive links are accessible and properly formatted.
* **Missing Data**: The script handles missing values by dropping affected rows.
* **Plot Display**: In some environments, use `plt.show()` to display plots.
* **Memory Issues**: For large datasets, consider processing data in chunks.

---

## Dependencies

* `pandas`: For data manipulation and analysis.
* `matplotlib`: For basic plotting functionality.
* `seaborn`: For statistical data visualization.
* `gdown`: For downloading Google Drive files.
* `os`: For directory and file operations.

---

## Author

Gaurav Adhikari

# Trading Data Analysis Project

This project analyzes trading performance data in correlation with market sentiment to identify patterns and insights for trading strategy optimization.

---

## Overview

This analysis combines trader transaction data with market sentiment classifications to explore:

* **Trading behavior patterns** across different market sentiments
* **Profitability analysis** by market conditions
* **Trade volume distribution** across sentiment categories
* **Daily trading trends** and performance metrics

---

## Features

* **Data Integration**: Merges trader data with sentiment analysis data.
* **Comprehensive Visualizations**: Generates multiple charts and plots for in-depth analysis.
* **Performance Analytics**: Analyzes PnL (Profit and Loss) across various market conditions.
* **Trend Analysis**: Identifies daily trading patterns and sentiment correlations.
* **Automated Setup**: Creates an organized directory structure for all outputs.

---

## Prerequisites

* Python 3.7+
* Google Colab environment (recommended)
* Internet connection for downloading datasets

---

## Required Libraries

The project relies on the following Python libraries:

* `pandas`
* `matplotlib`
* `seaborn`
* `gdown`

---

## Installation

1.  Clone or download the project files.
2.  Run the script in Google Colab or Jupyter Notebook.
    The script will automatically install required dependencies:
    ```bash
    pip install -q pandas matplotlib seaborn gdown
    ```

---

## Data Sources

The project uses two datasets hosted on Google Drive:

### Trader Data (`trader_data.csv`)

Contains trading records with timestamps, trade sides, sizes, and PnL.
**Fields include**: `Timestamp IST`, `Side`, `Size USD`, `Closed PnL`

### Sentiment Data (`sentiment_data.csv`)

Contains daily market sentiment classifications.
**Fields include**: `date`, `classification`

---

## Project Structure

After running the script, the following directory structure is created:

ds_Gaurav_Adhikari/
├── csv_files/
│   ├── trader_data.csv
│   ├── sentiment_data.csv
│   └── merged_data.csv
└── outputs/
├── trades_by_sentiment.png
├── profitability_vs_sentiment.png
├── volume_vs_sentiment.png
├── daily_trade_count_trend.png
└── daily_avg_pnl_trend.png


---

## Usage

1.  Run the complete script in Google Colab or Jupyter Notebook.
2.  **Data Download**: The script automatically downloads datasets from Google Drive.
3.  **Data Processing**: Cleans and preprocesses the data, handling missing values.
4.  **Analysis Generation**: Creates visualizations and saves them to the `outputs` folder.
5.  **Review Results**: Check the generated plots and the `merged_data.csv` dataset.

---

## Generated Visualizations

The script generates the following key visualizations:

1.  **Trades by Market Sentiment and Side**
    * **File**: `trades_by_sentiment.png`
    * **Description**: Count plot showing trade distribution across sentiment categories and trade sides (buy/sell).

2.  **Profitability vs Market Sentiment**
    * **File**: `profitability_vs_sentiment.png`
    * **Description**: Box plot analyzing PnL distribution across different market sentiments.

3.  **Trade Volume vs Market Sentiment**
    * **File**: `volume_vs_sentiment.png`
    * **Description**: Violin plot showing trade size distribution by market sentiment.

4.  **Daily Trade Count Trend**
    * **File**: `daily_trade_count_trend.png`
    * **Description**: Line plot tracking daily trading activity by sentiment over time.

5.  **Daily Average PnL Trend**
    * **File**: `daily_avg_pnl_trend.png`
    * **Description**: Line plot showing daily average profitability trends by sentiment.

---

## Key Analysis Points

* **Sentiment Impact**: Identifies how market sentiment affects trading behavior.
* **Risk Assessment**: Analyzes profitability patterns across different market conditions.
* **Volume Analysis**: Examines trade size variations with sentiment changes.
* **Temporal Patterns**: Tracks daily trading and profitability trends.

---

## Data Processing Steps

The project follows these data processing steps:

* **Data Loading**: Downloads and loads CSV files into pandas DataFrames.
* **Datetime Conversion**: Converts timestamp columns to proper datetime format.
* **Data Cleaning**: Removes rows with missing values to ensure data quality.
* **Data Merging**: Combines trader and sentiment data on date keys for integrated analysis.
* **Aggregation**: Creates pivot tables for comprehensive trend analysis.

---

## Output Files

* **Merged Dataset**: `merged_data.csv` - The combined trader and sentiment data.
* **Visualizations**: PNG files saved in the `outputs/` folder.
* **Console Output**: Data previews and processing status messages.

---

## Customization

To modify or extend the analysis:

* **Change Data Sources**: Update the Google Drive URLs in the script.
* **Modify Visualizations**: Adjust `matplotlib`/`seaborn` parameters for different chart styles or aesthetics.
* **Add Analysis**: Extend the script with additional metrics or visualizations.
* **Filter Data**: Add date ranges or other filtering criteria to focus your analysis.

---

## Troubleshooting

* **Download Issues**: Ensure Google Drive links are accessible and properly formatted.
* **Missing Data**: The script handles missing values by dropping affected rows.
* **Plot Display**: In some environments, use `plt.show()` to display plots.
* **Memory Issues**: For large datasets, consider processing data in chunks.

---

## Dependencies

* `pandas`: For data manipulation and analysis.
* `matplotlib`: For basic plotting functionality.
* `seaborn`: For statistical data visualization.
* `gdown`: For downloading Google Drive files.
* `os`: For directory and file operations.

---

## Author

Gaurav Adhikari
