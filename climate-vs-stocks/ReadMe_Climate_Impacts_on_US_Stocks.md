# Climate Impacts on U.S. Stocks

This project investigates the potential relationship between climate disasters and financial market performance. It merges NOAA climate event data with U.S. stock tickers to assess correlation trends and anomalies.

## 🎯 Objective

To explore whether major climate events influence U.S. stock returns and volatility on a sector or ticker level.

## 📁 Datasets

- NOAA Billion-Dollar Weather and Climate Disasters  
- Historical stock price data (multiple tickers)  
- Merged by event date and geographic region

## 🔧 Tools & Libraries

- `pandas`, `datetime` for event-window joining  
- `yfinance`, `sqlalchemy` for stock price queries  
- `matplotlib`, `seaborn` for financial trend plots

## 🔬 Key Techniques

- Joining time series by disaster date  
- Event-window market reaction plots  
- Sector filtering by SIC codes  
- Stock-level average return calculation

## 📊 Key Outputs

- Event-based return plots  
- Correlation tables  
- Disruption timelines and post-event rebound windows

## ▶️ How to Run

1. Ensure required CSVs and ticker list are available  
2. Load and run all cells to generate post-disaster return analytics  
3. Adjust event windows or ticker filters as needed
