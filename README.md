# Equinox Fenix ReadMe File

## Description

Equinox Fenix is a forex trading robot developed by Forex Robot Easy Team. This expert advisor is designed to analyze market conditions and identify potential trade opportunities. It enters trades based on the identified opportunities and manages them according to predetermined profit and loss targets.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/equinox-fenix-review-stable-long-lasting-forex-ea-strategy/). Please note that ForexRobotEasy is not the official developer of this product. This ReadMe file only provides a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Features

- Analyzes market conditions and identifies trade opportunities
- Enters trades based on the identified opportunities
- Manages open trades according to predetermined profit and loss targets
- Uses external input parameters to customize trading preferences

## External Input Parameters

- PreferredPairs: A comma-separated list of preferred currency pairs for trading (default: 'EURUSD,GBPUSD,AUDUSD,USDCAD,EURGBP,USDCHF,AUDCAD,EURAUD')
- RiskPercentage: Risk percentage per trade (default: 1.0)
- TakeProfitPercentage: Take profit percentage (default: 2.0)
- StopLossPercentage: Stop loss percentage (default: 1.0)

## Global Variables

- ticket: Order ticket (-1 if no trade is open)
- isTradeOpen: Flag to check if a trade is open (false if no trade is open)

## Functions

### OnInit()

This function is called during expert initialization. Any necessary initialization code can be added here.

### OnDeinit(const int reason)

This function is called during expert deinitialization. Any necessary deinitialization code can be added here.

### OnTick()

This function is called on every tick. It checks if a trade is already open and manages open trades or enters new trades based on market conditions.

### AnalyzeMarketConditions()

This function analyzes market conditions to identify potential trade opportunities. Any code to analyze market conditions should be added here. It should return true if a trade opportunity is identified and false otherwise.

### EnterTrade()

This function enters trades based on the identified opportunities. Any code to enter trades should be added here. It also sets stop-loss and take-profit levels for the trades.

### ManageTrades()

This function manages open trades. Any code to manage open trades should be added here. It checks if the predetermined profit or loss targets are reached and closes the trade if necessary.

### CloseTrade()

This function closes the open trade. It attempts to close the trade and updates the trade status accordingly.

### TradeProfit()

This function calculates the current trade profit/loss. It returns the sum of the trade profit, swap, and commission.

## Disclaimer

This code is provided as a sample and is not the official implementation of Equinox Fenix. ForexRobotEasy is not the official developer of this product. For the official developer and more information about this product, please use MQL5.

Please note that trading involves risks, and the use of this code or the Equinox Fenix robot does not guarantee profits. It is important to carefully analyze the market conditions and consider your risk tolerance before using this or any other trading system.

## License

This code is provided under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this code, but please include the original header and give credit to Forex Robot Easy Team.
