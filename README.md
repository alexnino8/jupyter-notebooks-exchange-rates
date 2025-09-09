This project was my first using jupyter notebooks. Inside the notebook (which is a bit messy) you can see that the goal is to convert a list of purchase amounts from EUR and GBP to USD and then export a new csv. 

The exchange rates had to be of a specific date so I used the Vatcomply API to get the exhange rate from that date and added the exchange rate column. Then I multiplied the amount times the exchange rate to a new amount_usd column. 

the output.csv is the first export but I noticed that the amounts were hard to read because it had no decimal places constraints, which I added for the second export which is rates_converted.csv