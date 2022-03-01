----
<p align="center">
  <img src="img/Cointegration.png" />
</p>
#### Introduction
Cointegration spread trading is a statistical arbitrage strategy for trading financial assets. You basicially trade two cointegrated assets, that is two assets that have the same price fluctuations and long term movement. But when they once in a while move apart from each they tend to revert back to the mean at some point. It's that knowledge you can use to your advantage.
Practically you buy one af the assets and sell the other, This way you can remove the risk of being affected by the general market movements, which is a huge advantage. 

In the past it was possible to use mean-reverting strategies to trade assets and you could be profitable. But as with most all trading strategies, as they are used by more and more people they loose their edge and stops being profitable. I don't expect this strategy to be higly profitable.
#### Goal
I want to investigate if using a mean-reverting strategy using cointegration can give any information about price movements in the traded assets. Any information we can derive from this strategy can be used as an factor in another larger model.

#### Conclusion
So far it hasn't been possible to get much edge in this strategy. That is, the different factors like Sharpe ratio and profit hasn't bee significant enough to prove that we can derive any useful information or edge in this strategy. There is however room for more investigation as it migt be possible to improve the strategy.

#### Challenges faced
In the first attempts to find the optimal entry and exit thresholds there was a problem with the thresholds being overfittet to the training dataset. Becasue as I testet the thresholds on our first testset (2020) the results were horrible. I investigated it and it turned out that the training set didn't fully reflect the parameters of the population. The original trainingset was on hourly data from 2016 to 2019 and it showed the best results with a windowsize of only 20. When I expanded the trainingset to hourly from 2010 to 2019 I got a windowsize of 150. 

![Graphs](img/Github_graphs.jpg)

Read more about the process in notebook

Quantconnetc code and backtestreport:</br>
https://www.quantconnect.com/terminal/processCache?request=embedded_backtest_905cedf89d97241c80b91e4301658356.html

*Note: There seems to be some differences between the optimal paramters calculated and the optimal parameters for backtest. This is an issue I'm pursueing at the moment. Project will be opdated with my findings.*

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTU4NDI4NDIwOSwxNDU2NTM4NTQ2LC0xND
k5NTI1Mjc3LDUyNjU5OTQ1NCwtNTQyODQzMjE4LDE3NzE5MDMw
ODEsMjAwMzg2ODY1MywxMjkxOTczMDIsMTg1NTY0OTg5NywxMz
M5NTU3MTczLDE5Njc5Mjc1NTQsMTEzMzU5MDc4MiwtMTQzMzc5
ODA3MSwtMTMxMzQzODE2Miw0NTg0NjI5NzIsLTEwMDMwODA2MT
IsLTM2ODE4NDEyOF19
-->