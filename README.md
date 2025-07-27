### Problem Statement

Let us define the temporary impact function gt(X) as the amount of slippage you incur if you place X orders at the current time t.

For this order book state, the best bid is $80.93, the best ask is $80.97, the spread is $0.04. The amount of orders in each limit order price is specified in
red (ask) and green (bid).

Let us suppose that we have S total amount of orders to be bought, you are given how many shares S to buy before market opens, and must buy exactly S shares by end of day. You are tasked with creating a strategy that is supposed to minimize the total temporary impact of the executed orders. Mathematically speaking, let gt(X) be the temporary impact function at some time t. Let us split the day into N trading periods. Let x ∈ RN be your allocation vector (we generally have to take integer quantities but real numbers are okay for now) where you choose to buy xi shares at the ith period. Given data for N = 390 (one minute trading window) and data for 3 stocks.

Please answer the following questions:

1. How do you choose to model the temporary impact gt(x)? For example, sometimes people try to ”linearize” the model gt(x) ≈ βtx. If yout hink linear models are gross oversimplifications, how would you model it? Please write a 1-2 page explanation on your model, using data from the 3 tickers provided. We understand that 3 tickers is not enough data so any valid reasoning/conclusions derived from these 3 tickers would be accepted. Please also attach a link to a python notebook or code (prefably uploaded on GitHub) where you conducted your analysis.
2. Formulate roughly but rigorously a mathematical framework / algorithm that gives us xi when we are at time ti. Make sure that P i xi = S. This should be relatively short, at most 2 pages. You don’t have to fully solve the problem, but a clear mathematical setup and discourse into the techniques + tools used to solve the problem would be sufficient
