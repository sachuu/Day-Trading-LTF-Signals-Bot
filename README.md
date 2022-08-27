# Day Trading LTF Signals Bot (PineScript)
------
![Screenshot](https://i.imgur.com/6J4ifi2.png)
## Setup
1. Navigate to TradingView.com
2. Select an asset and navigate to **advanced chart**
3. At the bottom of the page select **pine editor** and expand this section
4. Copy/paste **script.pine** into pine-editor
5. Select **Add to Chart** in the top right menu

**Note:**
*signals are ideal on the 15 min time frame*

## How it works
The signal looks for two conditions based on **VWAP** and **Stoch RSI**. 

VWAP represents the average price adjusted for volume. The script looks for when price crosses the VWAP trendline. Indicating a rapid spike in volume and price. VWAP helps indicate if price is undervalued or overvalued, a cross and break represents a potential shift in trend supported by volume. 

Stoch RSI gives a measurement based on the current, lows, and highs of the RSI based on a set number of periods (14 for this script). It also helps indicate when a stock is overbought or oversold. It tracks two values based on the highs and lows and when these values cross the second condition for a signal is given. Both the VWAP and Stoch RSI giving a positive signal in succession shows strong signs of a shift in momentum. 

## Roadmap

### Third confirmation
Pivot Points act as additional confirmation of a shift in trend. They act as support / resistance lines and a break or retest of one of these levels can serve as a third confirmation signal. 

Looking to add this as an additional condition for a signal in the future. For now these levels can added manually as an overlay with the following settings:

**Pivot Points Standard**
Type: *fibonacci*
Show historical pivots: *true*
Pivots Timeframe: *Daily*
Number Of Pivots Back: *15*

### Optimizing time periods for crypto market

Looking to backtest experimenting with adjusting the periods considered for Stoch RSI calculations. The 14 period standard being based on regular stock trading hours it would be interesting to see how adjustments can be made to optimize for crypto for example where markets are open 24/7. 

## Strategy
This strategy is inspired by the free trading resources published by @EmperorBTC. Please take some time to visit his page and find some great insights into trading

**Note** 
*All the information made available here is generally provided to serve as an example only, without obligation and without specific recommendations for action. It does not constitute and cannot replace investment advice*
