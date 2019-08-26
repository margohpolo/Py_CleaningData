# Py_CleaningData
Download from QuantConnect | Format for MT4 | Written in Python.

# Description
Data from QuantConnect is not compatible for uploading to MT4; therefore this bit of code was written to convert the formatting.

# Before
![Not even readable](https://github.com/margohpolo/Py_CleaningData/blob/master/csv_before.PNG)
Milliseconds Elapsed Since Midnight |Bid Rates: Open-High-Low-Close & Volume(0) | Ask Rates: Open-High-Low-Close & Volume(0)

# After
![Much better](https://github.com/margohpolo/Py_CleaningData/blob/master/csv_after.PNG)
Date | Time | Open-High-Low-Close & Volume(0)

# Afterthoughts
- Did not convert from server date and time (probably Cyprus) to local (Singapore). Bigger picture, though, may not matter.
- Could have found a solution to automate the formatting process, to loop through all the files in the folder. (Instead, manual input is required)
- My original intentions were to obtain more data, to vigorously backtest a trading bot I wrote in MQL4 language. I would have also uploaded MQL4 code for my automated trading strategy on MT4, but (a) running MT4 with over a decade of historical data causes it to constantly crash; & (b) said trading bot lost money in a horrendous manner when backtest period was longer than a couple of years.
- Nonetheless, learning how to format CSV data got me interested in Python.
