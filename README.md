# STOCK PRICE ANALYST

We need to add the stock that we want to run our analysis in the `config.json` file @two places.</br>
"new_stocks" is for all the newly added stocks, for which we would like to get the history added.</br>
"stocks" is for all the stocks on which the history is already run and we are running the daily analysis on these stocks.

## Installation

```bash
https://github.com/ShubhankarRaj/stock_price_analyst.git
```

## Usage

```
run requirements to install dependencies
```

To create the DB
```bash
python create_db.py
```
To create the TABLES
```bash
python create_table.py
```
To save history information in DB. This will take all the stock symbols from config db save the
history for them in ticker table
```bash
python orchestrator.py --hist
```
To save sentiments data in DB. 
This will take all the stock symbols from config db save the info for them in ticker table
```bash
python orchestrator.py --s_hist
```

To save info of everyday in DB. 
This will take all the stock symbols from config db save the info for them in ticker table
```bash
python orchestrator.py --info
```

To take a dump of DB  
This will take all the stock symbols from config db save the info for them in ticker table
```bash
python orchestrator.py --dump
```
