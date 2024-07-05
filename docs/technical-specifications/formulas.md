---
sidebar_position: 2
---

# Formulas

## Amount of shares to mint on deposit
$$
\begin{aligned}
    & a = \text{amount} \\
    & B = \text{balance of token before deposit in round } n \\
    & T = \text{total supply of shares in round } n \\
    & s = \text{shares to mint} \\
    & \frac{T + s}{T} = \frac{a + B}{B} \\
    & \text{if } T \neq 0 \text{ then } s = \frac{aT}{B} \\
    & \text{else } s = a
\end{aligned}
$$

where `s` is the amount of shares to be minted to depositor

## Amount of collateral to withdraw

### Instant & Standard Withdraw
They both will follow the same formula:
$$
\begin{aligned}
    & a = \text{amount} \\
    & B = \text{balance of token before withdraw (collateral amount)} \\
    & T = \text{total supply} \\
    & s = \text{shares to burn} \\
    & \frac{T - s}{T} = \frac{B - a}{B} \\
    & a = \frac{sB}{T}
\end{aligned}
$$

Where `a` is the amount of collateral to be returned back and `B` is the total amount of collateral in the round which includes the premium collected + collateral.

## Constants:
1. Deposit Phase: 2 hours
2. Options tokens expiry duration: 2 hours after being minted
3. Timeline of phases:
    1. t=0 to t=2hours - deposit phase
    2. t=2hours to t=4hours - active phase
    3. t>=4hours - execution phase
4. Amount of APT in one option token - 10 APT in 1 Options token.
5. Premium Price - 5 USDC
6. Performace Fee - 7.5% if the round is out-of-the-money. This fee will go to the Titus Finance account.
