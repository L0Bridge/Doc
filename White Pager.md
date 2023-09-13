# L0 Bridge
L0 Bridge is a decentralized cross-chain bridge based on L0 cross-chain technology, offering low fees, high security, and high flexibility.

## Low Fees
When using L0 Bridge for cross-chain transactions, users only need to pay minimal L0 gas fees and very low bridge fees, currently set at one hundred thousandth of the bridge amount. For certain specific currencies, fixed bridge fees can also be set, meaning that the bridge fee remains the same regardless of the size of the cross-chain amount.

## High Security
L0 Bridge is built on L0 cross-chain technology, which has been running securely and stably for several years without major security vulnerabilities. 

The L0 Bridge contract design is straightforward and has undergone multiple rounds of auditing by experienced developers in the crypto community. We believe this makes it more reliable than audit reports from most other institutions.

## High Flexibility
L0 Bridge supports the interoperability of all cross-chain currencies on the supported blockchains. When liquidity is insufficient on one chain, users can safely redeem funds from another chain.

# Liquidity added
## User adds on-chain liquidity
Users can add liquidity to any chain to obtain LPToken (Liquidity Providers Token).

LPToken is a net-value token whose value increases with the increase in handling fees.
## Liquidity redeem
Liquidity added on a specific chain can only be withdrawn on that chain.

By default, LPToken can be redeemed and converted into real Token. If liquidity is insufficient, it can also be redeemed as CPToken. CPToken can be cross-chained to other chains, and then the real Token can be redeemd from other chains.

# Cross-chain
## Cross-chain Registration
Only DAO can register cross-chain currency mapping.
## Review
If the currency addresses on both chains are the same, the review process can be omitted. Otherwise, the correctness of the address needs to be verified. The review process may differ depending on whether the currency already exists on both chains, and may be more complex or simpler.
## No need to register to cross-chain
If the target chain does not register the currency, the user will receive Custom-CPToken. Custom-CPToken is an ordinary token that can be used for transfer transactions, but it cannot be exchanged for a real Token on the target chain, nor can it cross to a non-source chain, that is, it can only go back and forth from there.
## When liquidity is insufficient
After cross-chain, if the liquidity is insufficient, the user will receive CPToken and cannot redeem it until the liquidity is sufficient. This kind of CPToken is different from the Custom-CPToken obtained across chains when not registered. It can be cross-chained to any registered chain and then redeem the real Token from these chains.

# Cross-chain Fees
## The fee consists of two parts
L0 gas fee + bridge fee
## Bridge fee
Can be fixed or proportional
### Bridge fee currency
What is collected is cross-chain currency.
### Fixed bridge fee
The fixed bridge fee needs to be set by the DAO. If there is no fixed bridge fee set, it will be charged according to a fixed ratio, and the rate will be as low as MultiChain.
### Security of fixed fee setting
The fixed fee setting has a safety protection mechanism and cannot exceed the maximum proportionally calculated amount. For example, if the maximum ratio is 1%, you cannot set a fixed fee of more than 1%.
### Proportional rate of bridge fee
The proportional bridge fee rate is set by DAO. If a certain currency does not set a fixed bridge fee, the cross-chain bridge fee will be charged in proportion.
### Security of proportional rate settings
The maximum proportional rate can only be set to 1%
### Bridge fee must be charged
If it is found that the amount of cross-chains is too small and the bridge fee cannot be charged, at least an unit fee will be charged.

## L0 Gas fee
There is no way to optimize the L0 gas fee charged by L0. It is a fixed fee set by L0 at some time.
## Fee Donation
Support project parties or other big players to donate cross-chain fees.

The donation is divided into two parts, the bridge fee donation and the L0 gas fee donation. 

Once donated, it cannot be returned.
### L0 gas fee donation
L0 Gas fee donation is used to launch cross-chain chains. eg: L0 gas fees donated in the arbitrum chain can only be used in arbitrum cross-chain, using L0's own subsidy mode.
### Bridge fee donation
The bridge fee donation is used to target chains. eg: The bridge fee donated in the arbitrum chain can only be used when crossing the chain to arbitrum, and it can only be in the cross-chain currency.

# Income Distribution
## Liquidity Rewards
### Reward users
Add liquidity users
### Liquidity reward source
A certain proportion of cross-chain bridge fees, the proportion can be adjusted by DAO. Currently 60%

##Project Party Income
### Source of income
A certain proportion of cross-chain bridge fees, the proportion can be adjusted by DAO. Currently 25%

## DAO income
### Source of income
A certain proportion of cross-chain bridge fees. The proportion can be adjusted by DAO. Currently 15%.

# DAO
## Configurable parameters
Income distribution ratio, default bridge fee ratio, fixed bridge fee, currency register, withdrawal of all liquidity of ReBase deflation currency

# Special attention
## Beware of deflation and inflation currencies
Deflation and inflation currencies are not within the scope of L0 Bridge support, but they have no impact on L0 Bridge. The L0 Bridge contract will calculate the actual amount received.
## Be careful with ReBase currencies
ReBase currencies is not within the scope of L0 Bridge support. The excess of ReBase does not affect user use, that is, the liquidity recorded in the contract is less than the real balance, and DAO can withdraw the excess.

ReBase deflation will affect the use of users. At this time, users cannot perform remove operations because the deflation will immediately affect the interests of other users. The liquidity of this currency can only be proposed by DAO and handed over to DAO for subsequent processing.
