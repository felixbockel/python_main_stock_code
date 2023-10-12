# python_main_stock_code

## Aim: 

### 1) Analyse historical data for the last 5 years from tickers US, Australia, ETFs and more. If tickers are no older than a year, will be neglected.
### 2) Select the most fitting tickers in terms of uptrending and reasonable low random variation for daily trading
### 3) interact with website to extract raw data and action buy or sell

## Code:

1) first script is python_extract_tickers: webscraping to get tickers from yahoo webpage
2) second are scripts that defines historical and price fluctuation and price data named python_historical_data_definition and python_price_fluctuation_noise_definition
3) third are scripts that run 2) script and include tickers named python_price_fluctuation_noise_main_script and python_us_historical_data_definition_main_script
   -> python_us1_historical_data_using_historical_definition and python_us_historical_data_complete_without_definition are pre stages of scripts above
4) fourth is a script that validates and runs 3) scripts in parallel mode cpu based named python_validate_historical_data_scripts_prep_daily_scripts (runs 3) in task manager and uses a fixed time to check whether scripts are finished) or python_validate_historical_data_before_running_daily_scripts (manages 3) scripts within the script)
5) fifth is a script that consists of 2 functions. first function adds extension to ticker that are chosen for daily trading. extension consists of full day of trading a day before that. second function combines historical_data and price_fluctuation_noise data and chooses the best tickers for daily trading. second function uses first function. the script is called python_choose_tickers_for_daily_trading_and_add_extension.
6) sixth is a script that defines statistic models that are used in the model script in 7). it is called python_statistic_definitions_for_model_script.
7) seventh script uses moving avg and savol statistical model to trend daily trading data that comes in one by one. It finds local max and min. forwards that information to script 8) to make a decision whether to buy or sell. this script is called python_statistical_model_trend_daily_data.
8) eigth script validates script 7) whether local max and min where found and when is the value set to buy or sell. This value is forwarded to scipt 9). This script is called python_validate_model_script_sell_or_buy.
9) last script is called python_webscraping_sell_buy_on_website and mainly used to interact with the website, therefore, it is always running. It uses information from script 8) when to buy and sell and insert this value into the website.
