# Bar Strength Divergence indicator for MT5

This code represents the Bar Strength Divergence indicator for MetaTrader 5 (MT5). It is used to identify divergence between price and the strength of the bars. The indicator calculates the bar strength for each candle and plots it on the chart.

## Indicator Parameters

- `resistanceLevel` (default: 1.0): The resistance level used to determine the bar strength.
- `supportLevel` (default: 0.5): The support level used to determine the bar strength.

## Indicator Buffers

- `barStrengthBuffer[]`: The buffer that holds the calculated bar strength values.

## Initialization Function

The `OnInit()` function is called when the indicator is initialized. In this function, the indicator buffer is set using `SetIndexBuffer()`, and the indicator label is set using `PlotIndexSetString()`.

## Calculation Function

The `OnCalculate()` function is called for each new tick received by the indicator. In this function, the bar strength is calculated for each candle. If the high of a candle is above the resistance level, the bar strength is increased by 1.0. If the low of a candle is below the support level, the bar strength is decreased by 1.0. The calculated bar strength values are then stored in the `barStrengthBuffer[]` buffer.

## Product Description

The Bar Strength Divergence indicator for MT5 is a powerful tool for identifying divergence between price and the strength of the bars. By analyzing the relationship between price levels and the resistance and support levels defined by the user, this indicator can help traders identify potential trend reversals or continuation patterns.

To use this indicator, simply install it on your MetaTrader 5 platform and apply it to your desired chart. The indicator will plot the bar strength values on the chart, allowing you to visually analyze the divergence between price and bar strength.

Please note that ForexRobotEasy is not the official developer of this product. We are providing this sample code as an example of how the indicator works. For detailed reviews and trading results of this product, please visit the official developer's website at [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-bar-strength-divergence-indicator-for-mt5/). To find the official developer of this product, please refer to the MQL5 website.
