## Content

[Farming on ETH](#farming-on-eth-chain)

[Providing Liquidity on Pancakeswap](#providing-liquidity)



## Farming on ETH-Chain

Farming on Jup(ERC20) is possible via farm on unicrypt

The devteam created a youtube video, so no need for a wall of text or pictures :)

It just has the original logo introduced:

[Buy, provide Liquidity and farm JUP](https://www.youtube.com/watch?v=9UMw3Q5R77w)



## Providing Liquidity and Farming/Staking on BS-Chain

#### Providing Liquidity

 You need to provide liquidity on the JUP/BNB-Pool Version 2 on [Pancakeswap](https://pancakeswap.info/token/0x0231f91e02debd20345ae8ab7d71a41f8e140ce7)

![pool](pics/bwjup_bnb_pool.png)

Don't worry if something like "The data on this site has only synced to Binance Smart Chain block 4917536 (out of 5497233). Please check back soon." appears on top of the side. It basically means that data is not accurate in this view, however the information of the jupitertoolkit bot is:

![toolkit_pancake](pics/jtk_pancake.png)

If you want to provide liquidity or trade, click the buttons on the right.

The bwJUP-Contract address is [0x0231f91e02debd20345ae8ab7d71a41f8e140ce7](https://www.bscscan.com/token/0x0231f91e02debd20345ae8ab7d71a41f8e140ce7)

If you click on "add Liquidity" the swap-app is loading and you should see this window:

![tokenimported](pics/imported_warning.png)

Check the contract-address and then click "understand" and "Continue".

You are here then:

![liq1](pics/pancake_liq2.png)

Now is a good time to select the right wallet-address. Open metamask (or any other suitable wallet) and select the account you have your BNB and bwJUP in, if it is not already selected.

The main thing on liquidity is, you have to provide the same value of both coins. If you put in 100$ of BNB, you need to add also 100$ of bwJUP.

Wait, on the screenshot above, there is no bwJUP selected, so lets add it:

![select_token_name](pics/select_token1.png) 

No bwJUP appears... if it does, select it, if not, put in the contract-address:

![select_token_address](pics/select_token2.png)

Now select it. 

As said, you need to add the same amount. The App automatically calculates the amount needed for the second token, if yo enter an amount on one of them:

![supply](pics/supply.png)

Here 0.1 BNB were put in and the system calculated 823.347 bwJUP. When you decided what you want to add, click "Supply", but remember, you need to have some small amount of BNB left to pay for the transactions.

![pool_tokens](pics/pool_tokens.png)

The number you see here is the Pool-Token. This is what you get in your wallet for providing the liquidity. Later, on a farm, you need to input these tokens. For now, you will just find that amount in the list of liquidity-providers on bscscan (we will see later). Click "Confirm Supply" and your wallet (here Metamask) should open up:

![confirm_tx](pics/confirm_tx.png)

This is the transaction that sends the tokens into the pool, click confirm and wait till it is done.

If it is not confirm supply but approve bwJUP, confirm it also and then you need to confirm supply after that .

When the transaction is done, you should find your amount of pool tokens you saw above in the contract for [PancakeSwap Liquidity Provider (LP) token](https://bscscan.com/token/0x6c7cdffa997f46598b9616bc0481372e45a00dc4#balances) that represents the bwJUP/BNB-Pool.





Now this Coins can be put into a farm to earn more rewards:

Swap it to mainnet on swap.jup.io. More details will follow.