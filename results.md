---
layout: page
title: Results
---

{:refdef: style="text-align: center;"}
![image-title-here](/img/backtest_summary.png){:class="img-responsive"}
{: refdef}

terative Training: the test set is predicted and trained sequentially and 
iteratively for each epoch. the objective is to let the model train on the 
recent samples in the past, such that the model could adapt to the changes 
in market environment.

## Non-Iterative Backtest Results
{:refdef: style="text-align: center;"}
![image-title-here](/img/usdjpy.png){:class="img-responsive"}
![image-title-here](/img/usdcad.png){:class="img-responsive"}
![image-title-here](/img/audusd.png){:class="img-responsive"}
![image-title-here](/img/eurusd.png){:class="img-responsive"}
{: refdef}

## Iterative Backtest Results
{:refdef: style="text-align: center;"}
![image-title-here](/img/usdjpy_iterative.png){:class="img-responsive"}
![image-title-here](/img/usdcad_iterative.png){:class="img-responsive"}
![image-title-here](/img/audusd_iterative.png){:class="img-responsive"}
![image-title-here](/img/eurusd_iterative.png){:class="img-responsive"}
{: refdef}