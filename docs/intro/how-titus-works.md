---
sidebar_position: 2
---

# How Titus Finance V1 works?

## Foundation
Titus Finanace operates Vaults with Covered Call startegy, where users deposit funds into vault. This funds are used to mint option tokens and list them for auction. Once auctioned, the amount collected is sent to vault as premium. If the options expire in-the-money, the buyers of auction make the profit and if the options expire out-of-the-moeney, the buyers make the loss.

## Lifecycle
1. Deposit period starts and is active for 2 hours.
2. Users deposit funds and get shares.
3. Deposit Period ends and keeper mints option tokens.
4. Option tokens are put on auction.
5. Buyer buys an option contract before expiry. This payment is sent to the vault.
6. On Expiry if
    1. ITM: Buyer gets the profit by selling part of the collateral deposited and returning remaining collateral back to vault.
    2. OTM: Buyer doesn't get anything and the collateral is returned back to vault in full.

### Functioning of options on Titus Finance:
Titus Finance will have a concept of rounds (r). Rounds represent distinct interval in which the options lifecycle will operate.

$$
\text{round} = k \quad \text{where} \quad 1 \leq k \leq n \quad \text{and} \quad k \in \mathbb{N}
$$

Where:
- `round` is the variable.
- `n` is the maximum value of the sequence.

This defines a sequence of integer values for `round` starting at 1 and ending at `n`.

### Updated Lifecyucle
1. Round N starts for t=0 to t=2hours
2. Users deposit during the deposit period and get shares.
3. Round N Deposit period ends and Round N+1 deposit period starts
4. Round N deposits are used to mint options token `On`.
5. `On` contracts are listed for sale.
6. Buyer buys the options and the amount used to purchase is sent to vault as premium for Round N.
7. On Expiry of `On` if
    1. ITM: Buyer gets the profit by selling part of the collateral deposited for `On` and returning remaining collateral back to vault.
    2. OTM: Buyer doesn't get anything and the collateral deposited for `On` is returned back to vault in full.
8. Repeat

## Phases of lifecycle:
1. Deposit Phase: Phase where users can deposit into a round to participate in minting of options token.
2. Active Phase: Phase where the options tokens are minted using the collateral deposited in a particular round and are available on auction.
3. Execution Phase: Phase where the options token is sold and the expiry date is in past. That is, t > expiryDate.

### Lifecycle segregated in Phases:
1. Round N starts for t=0 to t=2hours
2. Deposit Phase
    1. Users deposit during the deposit period and get shares.
3. Round N Deposit period ends and Round N+1 deposit period starts
4. Active Phase
    1. Round N deposits are used to mint options token `On`.
    2. `On` contracts are listed for sale.
    3. Buyer buys the options and the amount used to purchase is sent to vault as premium for Round N.
5. Execution Phase
    1. On Expiry of `On` if
        1. ITM: Buyer gets the profit by    selling part of the collateral     deposited for `On` and returning  remaining collateral back to vault.
        2. OTM: Buyer doesn't get anything  and the collateral deposited for `On`  is returned back to vault in full.
8. Repeat
