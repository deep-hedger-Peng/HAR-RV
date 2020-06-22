# Forecasting realized volatility in the SPY ETF with a simple Heterogenous AutoregRessive of Realized Volatility (HAR-RV) model
## Nathan Simonis
The goal of this notebook is to fit a simple HAR-RV model to forecast realized volatility in SPY.  This model assumes that investors with different time horizons percieve volatility differently [Muller et al.(1993)](https://ssrn.com/abstract=5370). 

Therefore, we will try to forecast the realized volatility in one day by taking into account the RV of the previous day, the previous week, the previous month, the closing price of an implied volatility index (VIX) and the daily traded volume in SPY.

The main papers followed to implement the simple HAR-RV are:
- Haugom, Erik and Langeland, Henrik and Molnár, Peter and Westgaard, Sjur, Forecasting Volatility of the U.S. Oil Market (January 29, 2014). Available at SSRN: https://ssrn.com/abstract=2691391
- Corsi, Fulvio, A Simple Long Memory Model of Realized Volatility (August 18, 2004). Available at SSRN: https://ssrn.com/abstract=626064 
