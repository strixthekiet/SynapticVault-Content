---
tags:
  - Math/statistic/time-series/Multiplicative-Model
---
# Multiplicative Model
### Description:
- Expressed as  $Y = T \times S\times R$ 
	- $S$ and $T$ are expressed as percentage
### Additive model forecasting with [[Seasonal Variation]]:
- When random is neglectible which means $R\approx 1, Y=T_{MA_n}*S$
	- where [[Time Series Trend|T]] is the [[Moving Average|MA]] of time frame $n$
		- which mean some S will also be missing
- Then seasonal variation of data point $Y_i, \ \ S_{Y_i}=Y_i/T_i$ 
	- ie, de-trended series
	- ex:

| Time | y   | T(MA_4) | $S$         |
| ---- | --- | ------- | ----------- |
| 1    | 92  |         |             |
| 2    | 115 |         |             |
| 3    | 104 | 103.2   | 1.007751938 |
| 4    | 131 | 103.6   | 1.264478764 |
| 5    | 74  | 104.8   | 0.70610687  |
| 6    | 94  | 105.4   | 0.891840607 |
| ...  | ... | ...     | ...         |
- Then for every group of data point, $G_{Y_i}=\{ Y_{i+an} \}$, there is a group of detrended series, $G_{S_i}=\{ S_{i+an} \}$ **(except the datapoints that dont have MA)**
	- ex: for MA-4, the first group, $G_{Y_1}=\{Y_1, Y_5, Y_9,...\}$ has detrended series $G_{S_1}=\{S_5, S_9,S_13...\}$
- Find the average detrended value for each of the group $G_S$, call it $\bar G_S$
- Minus $\bar G_S$ with an adjustment value ((sum-n)/n) to have the sum of all group's detrended value to number of group
	- The sum is **random component** if not 0
- Forecast the future [[Moving Average|MA]]:
	- Find the long term [[Time Series Trend|Trend]] of MA, $T_{MA}= (MA_{max}- MA_{min})/MA_n$
		- ie. trend of trend = Max MA - Min MA and divided by number of MA
	- Assume the long term trend hold, $MA_{i+1}=MA_i+T_{MA}$ 
- Then the next $Y, Y^*_{j}=MA_{j}*\bar G_{S_i}$  where $Y^*_{j}\in G_{Y_i}$
	- The next Y is the MA of that data point **multiply** the seasonal variant of that group
	- as same as $Y=T*S$
---