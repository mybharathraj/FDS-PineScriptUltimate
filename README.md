# FDS-PineScriptUltimate
All in One Pine Script For Use at STOCK Markets and Crypto Markets

### The first part of the code sets the indicator name and sets the lengthInput variable with an input for the length, which is a user-specified value with a minimum value of 2 and a default value of 150.

### The next part of the code defines the variables hi, lo, cl, op, and roc using the Simple Moving Average (SMA) of the high, low, close, and open prices, and the rate of change (ROC) of the close price, respectively.

### Then, the script calculates the lowest and highest values using the ta.lowest and ta.highest functions, which return the lowest and highest values of the lo and hi arrays, respectively.

### The following section defines the bool variables closeabove, closebelow, highabove, lowabove, openabove, paabovehigh, pabelowlow, and middle using conditionals that compare the close, high, low, and open prices to the corresponding cl, hi, lo, and op variables.

### The script then defines the colors bull, bear, neutral, standard, fillcolorbull, fillcolorbear, fillcolorneutral to be used for plotting later on.

### The next part of the code defines the hicolor, locolor, opcolor, clcolor, lowestcolor, highestcolor, and fillfinal variables, which will be used to determine the colors of the various plots based on the conditions specified in the conditionals.

### The script then plots the lowest and highest values using the plot function and sets the linewidth to 2.

### The following section defines the confirmOpenL and confirmOpenS variables, which indicate whether the close price is greater than or equal to the open price and whether the close price is less than or equal to the open price, respectively.

### The script then defines two variables isLong and isShort, and two signals long and short using conditionals that check if the close price is above or below the hi and lo values, respectively, and if the rate of change is positive or negative, respectively.

### The following section defines the ema10, sma20, ema34, sma50, sma200 variables using the Exponential Moving Average (EMA) and SMA of the close price, with the specified lengths of 10, 20, 34, 50, and 200, respectively.

### Finally, the script defines the previous values of each EMA and SMA using the [1] array index and calculates the final color for the candles using the yeslong and yesshort variables, which are defined using conditionals that compare the close price to the hi and lo values and whether the close price is above or below the long and short signals, respectively.


#### In this script, the color coding refers to the RGB values used to assign different colors to various elements in the chart that the script generates. For example, the colors "bull" and "deepbull" are defined as green (RGB values: 52, 120, 54) and a dark green (RGB values: 10, 241, 10), respectively. Similarly, "bear" and "deepbear" are defined as pink (RGB values: 244, 134, 143) and red (RGB values: 255, 0, 0), respectively.

#### These colors are used to represent bullish (positive) or bearish (negative) conditions in the chart. For example, if the close of the security being analyzed is above the Simple Moving Average (SMA) of the close, the color "bull" will be assigned to that bar. If the close of the security is below the SMA of the close, the color "bear" will be assigned to that bar.

#### Similarly, if the high of the security is above the SMA of the high, the color "hicolor" will be assigned the color "bull", otherwise it will be assigned the color "bear". The same logic applies to the colors "locolor", "opcolor" and "clcolor".

#### Finally, the color of the candles in the chart will be set based on the results of the analysis performed in the script, with the color "candlecolor" being set to one of the predefined colors, such as "bull", "bear", "neutral", "deepbull" or "deepbear".

#### In conclusion, the color coding in this script is used to visualize bullish and bearish conditions in the chart and to highlight when certain conditions are met.
