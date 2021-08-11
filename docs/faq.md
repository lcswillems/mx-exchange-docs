---
sidebar_position: 5
---

# FAQ

## What is the Maiar Exchange?

The Maiar Exchange is a DEX (Decentralized Exchange) with AMM (Automated Market Making) functions, deployed on the Elrond Network. It is the engine for DeFi products such as swaps, liquidity pools and yield farms.

## How do I connect my wallet to Maiar Exchange?

You can connect your wallet to the Maiar Exchange in three different ways: Maiar App, Ledger hardware wallet, keystore file (.json) + password via the Elrond Web Wallet.

## What are Swaps?

You can use a Swap to trade one token for another, based on the available token pairs. Because the Maiar Exchange is an AMM DEX, you will always be quoted a swap price based on the availability of tokens in a swap pool. Thanks to balancing mechanisms such as arbitrage, you will always receive a swap price that is close to the USD value of the swap, provided there is enough liquidity in the respective token pool.

## What are Liquidity Pools?

Liquidity Pools are smart contracts that hold the reserve of the two tokens for a particular Swap pair. Liquidity can be deposited in token amounts that are equal in USD value. The exchange automatically calculates this ratio based on the amount typed in by the user.

There is no limit to the amount of tokens that can be deposited in a liquidity pool - the more, the better. The proportion between the token amounts is always x * y = k - read the docs for an in-depth explanation.

## How to Add/Remove Liquidity 

You can add tokens to the available liquidity pools by selecting the corresponding pair, i.e. TKN1/TKN2. You can only add amounts of TKN1 and TKN2 that are equal in USD value.

After adding liquidity, you will receive a unique Liquidity Provider Token (LPT).

You can remove liquidity by giving back your LP token. It will be burned and you will receive the amount of TKN1 and TKN2 based on the current ratio between TKN1/TKN2 (this might be different than what is was initially), plus your share of the swap fees on the TKN1/TKN2 pair for the period when you have provided the liquidity. Please refer to the Impermanent Loss explanation to understand the potential risks involved with providing liquidity.

## What are the LP tokens?

An LP Token (Liquidity Provider token) keeps track of your added liquidity in a certain pool. It is a unique NFT that contains information about the amounts and time of deposit. It can be used to reclaim your added liquidity and it is burned in the process. Between the time you deposit liquidity and when you reclaim it, you can freely use the LP token to transfer it to another wallet or deposit it in a yield farm to get additional rewards. In the future you will be able to sell your LP tokens or leverage their value as collateral for borrowing money or other DeFi use-cases.

## What are Farms?

Farms generate yield for liquidity providers that stake the LP tokens. They are meant to incentivize long term liquidity by providing an additional revenue stream for providers. The rewards for farms are usually provided in MEX tokens, but special farms with dual token rewards can exist.

Liquidity providers can use farms by staking the LP tokens obtained from providing liquidity in a pool. After doing this, MEX rewards will periodically become available for harvesting. The rewards can be locked for 1 year for 2x APR.

## How to Use Farms?

You can deposit LP tokens in Farms to earn rewards by pressing the Stake button. For every token swap pair, a corresponding Farm is created. You can only stake TKN1/TKN2 LPT in the TKN1/TKN2 farm, for example.

Farms yield MEX rewards, which can be locked for 2x APR.

## How can I stake MEX?

You can stake MEX in a dedicated smart contract, listed in the “Farms” section, and earn rewards proportional to your deposited amount. This is a unique mechanism available only for the MEX token, which is part of the MEX value capture mechanisms.

## What is the difference between staking and farming?

Staking - Depositing MEX in the special MEX staking farm in order to earn rewards.

Farming - Also referred to as “yield farming”, the term refers to earning rewards for depositing LP tokens in their respective farms.

## What is Locked MEX (LKMEX)?

You can earn double APR on MEX farms if you choose to lock your rewards. When doing so, you will earn LKMEX token rewards.

LKMEX tokens always have the same value as MEX, but a different utility.

Utility:

- Staking LKMEX in the MEX Staking Farm for rewards
- Add liquidity to MEX pools*

*The deposited LKMEX are locked in a special smart contract that deposits the equivalent amount of unlocked MEX on the user’s behalf. The unlocked MEX comes from a dedicated MEX Liquidity Reserve.

**Each month (every 30 epochs) a new Locked MEX (LKMEX) is created that will start to be unlocked after 1 year (16.66% per month for the next 6 months).**

This means there are multiple Locked MEX tokens, each with different unlock schedules. There can be Locked MEX #10 which unlocks in October 2022, and Locked MEX 12 which unlocks in December 2022. Locked MEX #10 and Locked MEX #12 will always have the same value as the spot value of MEX, but they will be gradually unlocked according to the schedule.

## How many MEX tokens are there?

The MEX supply for Year 1 after launch will be 7,531,200,000 MEX tokens. The MEX token has an issuance mechanism that is designed to accelerate the Maiar Exchange adoption. It is countered by a MEX burning mechanism: 0.05% of all fees are swapped to MEX and then burned. This will lead to MEX becoming deflationary as its adoption broadens.

## What are the security funds used for?

Security is a top priority. A portion of the MEX supply has been set aside for funding periodic and exhaustive security audits, as well as future bounty programs, for all the Maiar Exchange components, from smart contracts to front-end components.

## What is the LKMEX time lock mechanism?

LKMEX tokens start unlocking 1 year after their creation, 16.66% each month, meaning it is fully unlocked after 18 months.

To keep the locking schedule simplified, LKMEX is always locked on the 1st of each month. This means that if you earn LKMEX on different days in March, for example, you will always get LKMEX tokens with the 01 March lock schedule.

## What is Wrapped EGLD?

The Maiar Exchange Smart Contracts work with ESDT tokens. EGLD is the native coin of the Elrond Network and needs to be wrapped as an ESDT token to work in Maiar Exchange.

Wrapped EGLD is used for each action that requires EGLD, such as swapping EGLD for another token, or depositing EGLD in a liquidity pool. The wrapping and unwrapping actions are automated by the interface.

## What is the Impermanent Loss (IL)?

Providing liquidity can be profitable, but you’ll need to keep the concept of impermanent loss (IL) in mind. IL describes the temporary loss of funds occasionally experienced by liquidity providers because of volatility in a trading pair.

The bigger the volatility, the more you are exposed to IL as there is an irresistible opportunity for arbitrage, because the price in the LP doesn’t reflect what’s going on. In this case, the loss means less dollar value at the time of withdrawal than at the time of deposit. Impermanent loss is one of the fundamental concepts, it’s something that anyone who wants to provide liquidity to AMMs should understand.

## What are Analytics?

The Analytics button is reserved for the section that provides additional information about the exchange and its token pairs, such as price charts, volume charts, and other pieces of useful information for traders. It will be made available in an upcoming release.