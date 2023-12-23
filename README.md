# Forex Robot Easy Team
## Ice Scalper Pro - Fully Automated Scalping Robot

Ice Scalper Pro is a fully automated scalping robot designed by the Forex Robot Easy Team. This robot utilizes a breakout strategy to capture profits from market movements. It is suitable for traders who prefer short-term trading and want to take advantage of volatile market conditions.

## How It Works
Ice Scalper Pro uses the MetaTrader 4 platform and requires the following libraries: Trade.mqh and PositionInfo.mqh. These libraries provide necessary functions for trading and managing positions. 

The robot is initialized with several variables:
- `lotSize`: Trading lot size. Default value is 0.01.
- `stopLoss`: Stop loss in pips. Default value is 20.
- `takeProfit`: Take profit in pips. Default value is 40.
- `slippage`: Allowed slippage in points. Default value is 3.

The main function `OnTick()` is executed on every tick. It checks if there are any open positions using the `Total()` function from the `positionInfo` object. If there are no open positions, it calculates the previous high and low using the `iHigh()` and `iLow()` functions. 

If the current price is above the previous high, a pending order to buy is placed using the `BuyStop()` function from the `trade` object. The parameters for the pending order are set based on the variables defined earlier.

If the current price is below the previous low, a pending order to sell is placed using the `SellStop()` function from the `trade` object. Again, the parameters for the pending order are set based on the variables defined earlier.

The `OnDeinit()` function is executed when the robot is stopped or removed from the chart. It closes any open positions using the `CloseAll()` function from the `trade` object.

## Product Description
Ice Scalper Pro is an advanced forex software developed by an independent developer. It is designed to automate the process of scalping, a popular short-term trading strategy. By utilizing a breakout strategy, this robot aims to capture profits from volatile market conditions.

Key Features:
- Fully automated scalping robot
- Uses breakout strategy to identify trading opportunities
- Customizable lot size, stop loss, take profit, and slippage parameters
- Compatible with MetaTrader 4 platform
- Suitable for traders who prefer short-term trading and want to take advantage of volatile market conditions

To learn more about Ice Scalper Pro, including detailed reviews and trading results, please visit the official developer's website [here](https://forexroboteasy.com/forex-robot-review/ice-scalper-pro-review-advanced-forex-software-breakout-strategy/). Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. For any further information or support, please contact the official developer through their website or refer to MQL5.
