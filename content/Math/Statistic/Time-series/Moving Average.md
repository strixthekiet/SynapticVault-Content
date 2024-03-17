---
tags:
  - Math/statistic/time-series
aliases:
  - MA
---
# Moving Average
### Description:
- A series of arithmetic averages over a given number of time periods. It is the estimate of the long run average of the variable.  
- Help smoothing out the data with less peaks and valley
	- large grouped data point will be more smooth
### Odd number of time periods MA:
- The average of any 3 data points becomes the value of the 2nd data point
### Even number of time periods MA:
- Say it is $n$ time periods 
- The average of any $2n$ ( ex 1 to 4) data points has position $2.5$
- Similarly for next 4 data points starting from $i+1$ (ex 2 to 5) becomes $1+2.5=3.5$
- Take average of the 2 averages is the value of position 3