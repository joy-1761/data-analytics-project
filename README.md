# data-analytics-project
This project contains a detailed statistical analysis of the performance of an automated trading algorithm, tested over 92 trades conducted in May–June 2020. The objective is to evaluate the profitability, risk profile, and behavioral patterns of the algorithm using walk-forward testing.
The analysis uses Python and popular data science libraries to clean the data, generate statistical summaries, visualize results, and run Monte Carlo simulations for future performance predictions.
Key Features
	•	Data Preparation & Cleaning
	•	Remove irrelevant or constant columns.
	•	Convert and format timestamps for analysis.
	•	Add derived metrics such as trade duration, profit per lot, trade direction, stop-loss/take-profit hits, and stop distance.
	•	Ensure data integrity via sanity checks (no missing or invalid values).
	•	Exploratory Data Analysis
	•	Time period of trading activity.
	•	Total profit and profit breakdown by market, direction, day of week, and trading hour.
	•	Distribution characteristics (mean, median, skewness, kurtosis) of Profit per Lot.
	•	Best and worst trades, average win/loss, win rate, loss rate, and profit/loss ratio.
	•	Trade Behavior Insights
	•	Frequency of consecutive losses and probability analysis.
	•	Trade duration analysis with empirical, exponential, and power-law distribution fits.
	•	Time spent in market by symbol.
	•	Method of trade closure (algorithm logic vs. stop-loss/take-profit triggers).
	•	Risk Analysis
	•	Maximum drawdown and drawdown duration.
	•	Time spent in drawdown as a percentage of the test period.
	•	Monte Carlo Simulations
	•	Simulate 100,000 possible account outcomes for the next 100 trades.
	•	Probability of making a profit.
	•	Best-case and worst-case scenario analysis based on historical trade distribution.
Technologies Used
	•	Python (pandas, numpy, matplotlib, scipy, datetime)
	•	Statistical Analysis & Probability Modelling
	•	Data Visualization
	•	Monte Carlo Simulation
Main Insights from This Dataset
	•	Win rate: ~40%
	•	Average win per trade: 17.34 (per 0.01 lot)
	•	Average loss per trade: -10.84 (per 0.01 lot)
	•	Profit/Loss ratio: 1.6
	•	Maximum drawdown: 243.01 zł over ~4 days
	•	Probability of profit over the next 100 trades (simulation): ~56.63%
Repository Contents
	•	`Trading-Results-Analysis.ipynb` / `.py` – Jupyter notebook or Python script with full analysis.
	•	`/img/` – Generated charts and figures.
	•	`OrdersReport.csv` – (Optional) Source trade dataset (not included here due to privacy).
	•	`Trading-Results-Analysis.pdf` – Complete written report.
How to Use
	1.	Clone the repository.
	2.	Install requirements from `requirements.txt`.
	3.	Add your own `OrdersReport.csv` or use the existing cleaning/analysis functions on similar trading datasets.
	4.	Run the notebook/script to generate statistics and visualizations for your backtests.
