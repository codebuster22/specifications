---
sidebar_position: 1
---

# ELI5

## Explain me options like I'm 5.

### Options as toys
Let's imagine you have a toy that you really like, but instead of buying it now, you make a special deal with a friend. This deal gives you the choice to buy the toy later at a price you both agree on today. There are two kinds of these special deals, called "options":

1. **Call Option**: This is like telling your friend, "I want to have the option to buy this toy from you later for $10." To make this deal, you pay your friend a small amount of money, let's say $1, called the "premium." If you see that the toy's price goes up to $15 at the store, you can still buy it from your friend for $10 and save $5. But if the toy's price goes down to $5, you don’t have to buy it from your friend. You can just get it from the store for the cheaper price. However, you don't get your $1 premium back.

2. **Put Option**: This is like telling your friend, "I want to have the option to sell you this toy later for $10." Again, you pay your friend a small amount of money, let's say $1, called the "premium." If the toy's price goes down to $5 at the store, you can sell it to your friend for $10 and make $5. But if the toy’s price goes up to $15, you don’t have to sell it to your friend. You can sell it at the higher price in the store. However, you don't get your $1 premium back.

In both cases, having the option is valuable because it gives you a choice, but it doesn’t force you to do anything. The $1 premium is like paying for a special ticket that lets you decide later if you want to use the deal or not. If the deal works out for you, you can use it and make a profit. If it doesn’t, you lose just the $1 premium you paid. That’s how options work!

### Options as Bets

**Call Option (Bet on the Price Going Up):**

1. **Your Bet:** You bet that the price of the asset will go above a certain price (X).
2. **Friend's Bet:** Your friend bets against you.
3. **Cost of the Bet (Premium):** You pay your friend a small amount (Y), which is the premium for this bet.
4. **Outcome if Price Goes Above X:** If the asset's price goes above X, you win the bet. You can buy the asset at the agreed price (X), even though it's worth more in the market. This allows you to make a profit because you can immediately sell it at the higher market price.
5. **Outcome if Price Stays Below X:** If the asset's price does not go above X, you lose the bet. You don't have to buy the asset, but you lose the premium (Y) you paid your friend.

**Put Option (Bet on the Price Going Down):**

1. **Your Bet:** You bet that the price of the asset will go below a certain price (X).
2. **Friend's Bet:** Your friend bets against you.
3. **Cost of the Bet (Premium):** You pay your friend a small amount (Y), which is the premium for this bet.
4. **Outcome if Price Goes Below X:** If the asset's price goes below X, you win the bet. You can sell the asset at the agreed price (X), even though it's worth less in the market. This allows you to make a profit because you can sell it for more than the market price.
5. **Outcome if Price Stays Above X:** If the asset's price does not go below X, you lose the bet. You don't have to sell the asset, but you lose the premium (Y) you paid your friend.

### Summary

- **Call Option:** You bet the asset's price will go up. If you're right, you buy the asset at a lower price and can sell it for a profit.
- **Put Option:** You bet the asset's price will go down. If you're right, you sell the asset at a higher price and can buy it back cheaper for a profit.
- **Premium:** The small amount you pay to your friend to make the bet, which you lose if your bet is wrong.

In both cases, the premium is like the cost of placing the bet, and the outcome depends on whether the asset's price moves as you predicted.

## In-the-money and Out-of-the-money.

### Call Option (Bet on the Price Going Up)

**In-the-Money (ITM) for Call Options:**
- **Explanation:** Your call option is "in-the-money" if the current price of the asset (toy) in the market is higher than the agreed price (X) at which you can buy it from your friend.
- **Example:** You have the option to buy the toy for $10 (X). If the toy is now selling for $15 in the store, your option is in-the-money because you can buy it for $10 from your friend and immediately sell it for $15, making a $5 profit.

**Out-of-the-Money (OTM) for Call Options:**
- **Explanation:** Your call option is "out-of-the-money" if the current price of the asset (toy) in the market is lower than the agreed price (X) at which you can buy it from your friend.
- **Example:** You have the option to buy the toy for $10 (X). If the toy is now selling for $5 in the store, your option is out-of-the-money because it would be cheaper to buy the toy directly from the store than to use your option.

### Put Option (Bet on the Price Going Down)

**In-the-Money (ITM) for Put Options:**
- **Explanation:** Your put option is "in-the-money" if the current price of the asset (toy) in the market is lower than the agreed price (X) at which you can sell it to your friend.
- **Example:** You have the option to sell the toy for $10 (X). If the toy is now selling for $5 in the store, your option is in-the-money because you can buy the toy for $5 and sell it to your friend for $10, making a $5 profit.

**Out-of-the-Money (OTM) for Put Options:**
- **Explanation:** Your put option is "out-of-the-money" if the current price of the asset (toy) in the market is higher than the agreed price (X) at which you can sell it to your friend.
- **Example:** You have the option to sell the toy for $10 (X). If the toy is now selling for $15 in the store, your option is out-of-the-money because it would be better to sell the toy directly in the store for the higher price than to use your option.

### Summary

- **Call Option:**
  - **In-the-Money:** Market price > Strike price (X)
  - **Out-of-the-Money:** Market price < Strike price (X)
- **Put Option:**
  - **In-the-Money:** Market price < Strike price (X)
  - **Out-of-the-Money:** Market price > Strike price (X)

This way, you can see how "in-the-money" and "out-of-the-money" apply differently to call and put options based on whether the market price is above or below the agreed strike price.

## Resources:
