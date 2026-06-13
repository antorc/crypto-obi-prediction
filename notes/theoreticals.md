# Root Question:
> "If I look at the buyers and the sellers, can I guess which way the price moves in the next fraction of a second, and if I tried to trade on that guess, would i make money after costs?"

Breaking it down:
Given a certain number of buyers at price X, lot size Y, and 
a certain number of sellers at price A, lot size B,
can i predict which way the price will move next?

# The Order Book

## Limit Order Book
In the crypto market, a single market price does not exist, why?
Instead, they run **limit order books**

## Bids, Asks & Spreads
- **Bid** — an order to *buy*
	- "I want to buy BTC at price X"
	- Sits *below* the current price, waiting to be filled
	- If a bid were above the current price, it would already have been matched by an ask
- **Ask** — an order to *sell*
	- "I want to sell BTC at price X"
	- Sits *above* the current price
	- If an ask were below the current price, it would already have been matched by a bid
- Each entry consists of:
	- **Price**
	- **Size** — how much

The **highest bid** is the buy order closest to the current price.
The **lowest ask** is the sell order closest to the current price.

```
Ask3
Ask2
Ask1   ← Best Ask (lowest)
------- Current Price -------
Bid1   ← Best Bid (highest)
Bid2
Bid3
```

Together, the highest bid and lowest ask form the **BBO (Best Bid and Offer)**.

Spread = Best Ask(Lowest Price) - Best Bid(Highest Bid)
→ the "price of immediacy": what it costs to trade *now*.

## Mid Price
Mid price "the price" = (Best bid + Best ask)/2

## Market & Limit Orders
- **Limit order** — "buy/sell, but only at this price or better"
	- Sits in the book and waits
	- → *provides* liquidity
- **Market order** — "buy/sell right now at whatever is available"
	- → *consumes* liquidity

# Running To Do/Questions:
- Why does a single market price not exist, is it due to decentralisation? What about centralised exchanges?
- What is the point of mid price? Is it the price at which a market order is filled?
- Order book imbalance
- Spots & Perpetuals

