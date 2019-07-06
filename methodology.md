---
layout: page
title: Methodology
---

---

#### Input Pre-processing
* Tick data of `USDCAD`, `USDJPY`, `EURUSD`, `AUDUSD`
* Data Period: `01-Jan-2005` to `18-May-2019`
* Ticks are resampled per 1000-BidVolume, and Bid prices are used to construct the OHLC bar in each timestep

{:refdef: style="text-align: center;"}
![image-title-here](/img/1000-volume-resampled-ohlc.png){:class="img-responsive"}
{: refdef}

---

#### Features Generation
Momentum and pattern indicators are generated using TALib, a popular library for technical analysis.

For each momentum indicator, the following resolutions are generated: [1min, 5min, 15min, 30min, 1H, 3H, 6H, D]
* Total Number of Pattern Detectors Available = 61
* Total Number of time-resampled OHLC ([1min, 5min, 15min, 30min, 1H, 3H, 6H, D]) = 8
* Therefore, the total number of patterns features generated = 61 x 8 = 488

{:refdef: style="text-align: center;"}
![image-title-here](/img/pattern_analysis.png){:class="img-responsive"}
![image-title-here](/img/momentum_indicators.png){:class="img-responsive"}
{: refdef}

---

#### Features Selection
* Each timestep has 503 features which is impractical due to machine resource restriction. 
* Random forest algorithm is applied to filter unimportant features to reduce the input dimension (number of features)
* The main idea of random forest is to construct a multitude of decision trees at training time. The more times a feature is being referenced in the decision trees, the more important the feature is

{:refdef: style="text-align: center;"}
![image-title-here](/img/random-forest.png){:class="img-responsive"}
{: refdef}