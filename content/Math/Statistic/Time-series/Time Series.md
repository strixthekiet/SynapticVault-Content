---
tags:
  - Math/statistic/time-series
---
# Time Series
### Description:
- Has:
	- $Y$ is the actual time series  
	- $T$ is the trend series  
	- $S$ is the seasonal component
	- $R$ is the random component (can be assumed to be negligible)
### Time Series Models:
- A time series model can be expressed as some combination of these four components.
### Types of models:
- 2 models that are commonly associated with time series: 
	- [[Additive Model]] 
	- [[Multiplicative Model]] 
- The multiplicative model is **better** than the additive model for forecasting **when the [[Time Series Trend]] is increasing or decreasing over time**
- The additive model suffers from the somewhat unrealistic assumption that the components are independent of each other. 
- In most instances, movements in one component will have an impact on other components.
- The multiplicative model is often preferred. 
	- It assumes that the components interact with each other and do not move independently. 
- Since extrapolation is based on historical data alone, and does not include effects of developments, it can be used for short-term forecasts only for specific areas, where no untypical developments are expected.  
### Components
- [[Time Series Trend]]
- [[Seasonal Variation]]
- [[Cyclical Variation]]
	- Many variables often exhibit a tendency to fluctuate above and below the long-term trend over a long period of time. 
	- They cover much longer time periods than do seasonal variations.  
- [[Random Variation]]
	- Caused by unusual and unexpected occurences producing movements which have no discernible pattern. 
	- These movements are unique and unlikely to reoccur in similar fashion. 
	- They can be caused by events such as wars, floods, earthquakes, political elections, or oil embargoes.  
### [[Deseasonalization]]