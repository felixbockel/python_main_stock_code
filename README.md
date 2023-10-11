# python_main_stock_code

1) first script is python_extract_tickers: webscraping to get tickers from yahoo webpage
2) second are scripts that defines historical and price fluctuation and price data named python_historical_data_definition and python_price_fluctuation_noise_definition
3) third are scripts that run 2) script and include tickers named python_price_fluctuation_noise_main_script and python_us_historical_data_definition_main_script
   -> python_us1_historical_data_using_historical_definition and python_us_historical_data_complete_without_definition are pre stages of scripts above
4) fourth is a script that validates and runs 3) scripts in parallel mode cpu based named python_validate_historical_data_scripts_prep_daily_scripts and sequential python_validate_historical_data_before_running_daily_scripts
5) fifth is a script that checks 



python_choose_tickers_for_daily_trading_and_add_extension
python_extract_tickers
python_historical_data_definition
python_price_fluctuation_noise_definition
python_price_fluctuation_noise_main_script
python_statistic_definitions_for_model_script
python_statistical_model_trend_daily_data
python_us1_historical_data_using_historical_definition
python_us_historical_data_complete_without_definition
python_us_historical_data_definition_main_script
python_validate_historical_data_before_running_daily_scripts
python_validate_historical_data_scripts_prep_daily_scripts
python_validate_model_script_sell_or_buy
python_webscraping_sell_buy_on_website


python_choose_tickers_for_daily_trading_and_add_extension
# first function adds extension to ticker that are chosen for daily trading. extension consists of full day of trading a day before that. 
# second function combines historical_data and price_fluctuation_noise data and chooses the best tickers for daily trading.
# second function uses first function.



python_statistic_definitions_for_model_script
# python all definitions to run statistical models for model script

python_statistical_model_trend_daily_data
# moving avg and savol statistical model to trend daily trading data that comes in one by one. It finds local max and min. forwards that information to another script named “” to make a decision whether to buy or sell. 

python_validate_historical_data_before_running_daily_scripts
# validate_historical_data_before_running_daily_scripts


python_validate_model_script_sell_or_buy
# validate model script whether buy or sell need to happen.

python_webscraping_sell_buy_on_website
# python webscraping sell and buy on website. use summarized data consisting of historical and price fluctuation and noise data to be able to determine when to buy and sell. use this information to insert that value and price into website automated.


