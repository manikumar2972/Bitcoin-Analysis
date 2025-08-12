# Trader Performance vs Market Sentiment

This project explores the relationship between trader performance (`Closed PnL`) and overall market sentiment using historical trading data and the Fear & Greed Index.

## 📂 Dataset
- **historical_data.csv** – Contains trader performance data with timestamps and `Closed PnL` values.
- **fear_greed_index.csv** – Contains daily market sentiment classifications (Extreme Fear, Fear, Neutral, Greed, Extreme Greed).

## 🔄 Data Processing
1. Load the datasets with **Pandas**.
2. Convert timestamp columns to date format.
3. Merge the datasets on the `date` column.
4. Map qualitative sentiment to numerical values:
   - Extreme Fear → -2  
   - Fear → -1  
   - Neutral → 0  
   - Greed → 1  
   - Extreme Greed → 2

## 📊 Analysis
- **Average PnL by Market Sentiment**:  
  Bar chart visualizing the mean `Closed PnL` for each sentiment classification.
- **Correlation Analysis**:  
  Pearson correlation between numerical sentiment score and `Closed PnL`.

## 📈 Output Example
- **Bar Chart**: Displays how average trader performance varies with sentiment.
- **Correlation Value**: A numeric measure indicating whether sentiment positively or negatively impacts performance.

## 🛠️ Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**

