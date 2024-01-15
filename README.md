# Price Action Sketcher ReadMe

This is a code file for the Price Action Sketcher trading strategy. The strategy is designed to analyze price action and generate trade signals based on the analysis. The code provided here serves as an example of how the strategy can be implemented in the MQL5 language.

## Constants

The code includes several constants that can be adjusted to suit individual trading preferences:

- `MIN_ACCOUNT_SIZE`: This constant represents the minimum required account size for the strategy to be executed. It is currently set to 500.0, but can be modified as needed.

- `TRADING_HOURS_START` and `TRADING_HOURS_END`: These constants define the trading hours during which the strategy will be active. They are currently set to 15 and 32 respectively, adjusted for GMT 3 timezone. Traders can adjust these values to match their preferred trading hours.

## Structures

The code includes a structure called `TradeSignal` which represents a trade signal generated by the strategy. It contains the entry price, stop loss level, and take profit level for a potential trade.

## Price Action Sketcher

The `OnTick` function is the main function that drives the Price Action Sketcher strategy. It checks if the current time is within the specified trading hours and generates trade signals accordingly using the `GenerateTradeSignal` function. If a valid trade signal is generated, the `ExecuteTrade` function is called to execute the trade.

## Price Action Analysis Function

The `GenerateTradeSignal` function is responsible for performing price action analysis and identifying potential trade opportunities. Traders can modify this function to suit their own price action analysis techniques.

## Entry and Exit Signals Functions

The `ExecuteTrade` function executes a trade based on the generated trade signal. Traders can customize this function to include their own trade execution logic.

## Risk Management Functions

The `CalculatePositionSize` function calculates the position size based on the stop loss level. Traders can modify this function to implement their preferred risk management strategies.

## Trade Monitoring Functions

The `OnTrade` function is responsible for monitoring open trades, tracking performance, and providing real-time updates. Traders can customize this function to include their own trade monitoring and performance tracking logic.

## Helper Functions

The `IsTradingHours` function checks if the current time is within the specified trading hours. It is used in the `OnTick` function to determine whether to execute the strategy or not.

Please note that Forex Robot Easy is not the official developer of this product. This code is provided as a sample implementation of the Price Action Sketcher strategy. For detailed reviews and trading results of the official product, please visit [Forex Robot Easy's Price Action Sketcher Review](https://forexroboteasy.com/forex-robot-review/price-action-sketcher-review-65-roi-forex-software/). To find the official developer of this product, please refer to MQL5.
