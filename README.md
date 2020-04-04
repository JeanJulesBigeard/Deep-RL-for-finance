# Deep-RL-for-finance

Why?

- No need for mathematical models.
- No need to hand-code trading strategies.

Just need to train your RL algo to optimize the metric of your choice (ex: Net profit, Risk-Adjusted return).

Simulated environments can simulate:

- Transaction fees
- Network latences
- Liquidity
- Other traders
- Different market conditions 
(...)

Goal: Learning the number of stocks to buy, sell and hold at each transaction.

Optimal liquidation problem: Assume that you have a certian number of stocks that you want to sell within a given time frame. Taking into account the costs arising from market impact and a trader's risk aversion, the goal is to create a trading list that sells all the stocks, within the given time frame, such that the total cost of trading is minimized.

1-/ `Almgren and Chriss Model.ipynb`: Almgren and Chriss Model for optimal execution of portfolio transactions, assuming permanent and temporary market impact functions are linear function of the trading rate and that the stock price followed a discrete random walk. It is a nice benchmark to compare our RL model.

2-/ `Trading Lists.ipynb`: See how trading lists vary depending on your initial trading parameters and how to implement a trade list in the simulated trading envirenment.

3-/ `Efficient Frontier.ipynb`: Explanations on the Expected Shortfall (E(x)) and the Variance of the Shortfall (V(x)) used to minimized the utility function (U(x) = E(x) + V(x)) where lambda corresponds to the trader’s risk aversion. .

4-/ `DRL.ipynb`:  Deep Reinforcement Learning for optimizing the execution of large portfolio transactions.
