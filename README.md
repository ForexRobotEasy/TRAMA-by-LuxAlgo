# TRAMA by LuxAlgo

TRAMA is a custom indicator developed by LuxAlgo. It is designed to provide reliable forex signals by using a non-repainting algorithm. This indicator calculates the TRAMA values based on the input parameters and the price data. The TRAMA values are then used to generate the main line buffer, which can be used for trading decisions.

## Indicator Input Parameters

- `period`: The period used for calculating the TRAMA values. The default value is 14.

- `buffer_shift`: The number of bars to shift the main line buffer. The default value is 1.

## Indicator Buffers

- `tramaBuffer[]`: The buffer that stores the TRAMA values.

- `mainLineBuffer[]`: The buffer that stores the main line values.

## Indicator Initialization

The `OnInit()` function is responsible for initializing the indicator. It sets the indicator buffers and label.

## Indicator Calculation

The `OnCalculate()` function is called for each bar to calculate the indicator values. It first checks if there is enough data available to calculate the TRAMA values. If not, it returns 0.

For each bar, the function calculates the TRAMA value by summing the closing prices of the previous `period` bars and dividing the sum by `period`. The TRAMA value is then stored in the `tramaBuffer`. 

The main line buffer is calculated by shifting the TRAMA values by `buffer_shift` bars. If the current bar index is greater than or equal to `period + buffer_shift`, the TRAMA value is stored in the `mainLineBuffer` at the corresponding index minus `buffer_shift`.

The function returns the total number of calculated bars.

## Product Description

TRAMA by LuxAlgo is a reliable forex software that utilizes a non-repainting indicator to generate accurate trading signals. The indicator calculates the TRAMA values based on the specified period and price data. These values are then used to generate the main line buffer, which can be used for making informed trading decisions.

The TRAMA indicator is easy to use and can be applied to any forex chart. It provides clear and precise signals, allowing traders to enter and exit trades with confidence. The non-repainting algorithm ensures that the signals remain reliable and accurate, eliminating false signals and increasing profitability.

Please note that ForexRobotEasy is not the official developer of this product. We provide this sample code as an example of how the TRAMA indicator works. To find the official developer of this product and access detailed reviews and trading results, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/trama-by-luxalgo-review-reliable-forex-software-with-non-repaint-indicator/).

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/trama-by-luxalgo-review-reliable-forex-software-with-non-repaint-indicator/).
