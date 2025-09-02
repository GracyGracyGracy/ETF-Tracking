# ETF-Tracking
Open-End Fund's automatic crawler and data analysis

# Function
crawl data from JISILU.CN

calculate every-day ETF Assets Under Management change from Shares and Net Asset Value

calculate Cumulative Change in Assets Under Management over Multiple Days

organize data into Excel for subsequent data visualization

# Instruction
Ensure that manual_index_data and etf_data1 are located in the same directory as the crawler code. 

On the initial execution of this code, ensure first_day_shares is in the same directory as the crawler code. After the first run, relocate first_day_shares to a different directory (avoid subsequent interruption).

Results will be outputted to etf_data1 folder.

Recommend-Schedule the code with the Windows Task Scheduler or Linux cron if needed

Recommend-For AUM-filtering results, include that day's AUM column to the latest output for filtering (use the latest daily NAV*Shares to compute AUM), ensuring AUM aligns with Index column.

# Library
Built-in Python Libraries

time, os, datetime, logging

Third-Party Libraries

requests, pandas, openpyxl
