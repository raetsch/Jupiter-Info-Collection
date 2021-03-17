# Gateways to swap JUP between the different chains

as we all (should) know, Jup is available on 3 chains currently:

- native JUPChain (Mainnet, where the announced dApps will run)
- ETHChain as ERC20 JUP (a pitty, should be wJUP)
- BS-Chain as BEP20 bwJUP (binance wrapped Jupiter - yeah :) )

now, to swap your coins to the different chains, there are gateways in place. The purpose of this info is to show how you can swap, what costs you have and if it is manually or automated.

There are 4 possibilities currently:

- Mainnet to bwJUP
- bwJUP to Mainnet
- ERC20 JUP to bwJUP
- bwJUP to ERC20 JUP

The possibility to swap Mainnet to ERC20 is not longer active, because of the high fees on ETH-Chain

## Swap Mainnet to bwJUP

By the time writing, this is done manually.

There is a blog article on jupiter homepage: [Blog MAinnet to BSC](https://gojupiter.tech/jupiter-main-to-erc20/). It is rather short but contains two important things:

-  **[JUP-V5K2-269Z-QHGN-FSFT8](https://jupitertoolkit.com/explorer/address/JUP-V5K2-269Z-QHGN-FSFT8)**. This is the gateway address for native JUP. So if you want to swap, send your JUP to this address 
- Where should the bwJUP be sent to? Put the address as a message  into your tx

![image-20210317224018838](C:\Users\hk\AppData\Roaming\Typora\typora-user-images\image-20210317224018838.png)

you have to tick "Add a Message?" to add your BSC-Address, calculate fee, enter your passphrase and good to go!

You can now head over to [jupitertoolkit explorer](https://jupitertoolkit.com/explorer/address/JUP-V5K2-269Z-QHGN-FSFT8) and see if your tx came in.

After it is processed (as said manually currently), you should see the outgoing tx on the bs-chain on [bscscan bwJUP contract](https://bscscan.com/address/0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca#tokentxns)

When the tx is there, you should see the coins in your wallet.



## bwJUP to Mainnet

tbd.

basically the way backward, but has to be confirmed.



## ERC20 JUP to bwJUP

this Gateway is automated.

The trick here is, bsc is a copy from ETH (well, more or less). The good thing on that. Your private key is the same on ETH as on BSC, so if you have an address on ETH, it is the same on BSC. This is the way how the automated gateway works. Incoming tx from the ETH-Network are sent out over BSC back to the same address you sent it on ETH-Network!

An example:

![image-20210317232235147](C:\Users\hk\AppData\Roaming\Typora\typora-user-images\image-20210317232235147.png)

Somebody sent 46487 ERC20 JUP to the Gateway (you notice the "IN").

![image-20210317232354383](C:\Users\hk\AppData\Roaming\Typora\typora-user-images\image-20210317232354383.png)

Here, on BSC, the tx was sent out - to the same Address!

So, how does it work?

There is again a blog entry for that: [swap ERC20 to BEP20](https://gojupiter.tech/erc20-jup-to-bwjup-bsc-version/). We get the Gateway address from there: **0x34fbBB37Eb4f50f447E736E7B771bd3aD20C41cA**.

Open your wallet, click send and enter the receipient (the gateway address).

![image-20210317232805351](C:\Users\hk\AppData\Roaming\Typora\typora-user-images\image-20210317232805351.png)

After you entered the address, you can choose what to send (standard is ETH). Select JUP, Enter the amount you want to swap and select the tx-speed (no need to go higher than average).

**And this is the cost for this swap** - you have to pay the ETH tx-fee, which is rather high. You can lower it by selecting a slower speed (means you pay less for the tx and therefore miners will add it later) or monitor the gasprices (for example on gasnow.org) and wait until it gets cheaper.



When it arrives at the gateway, it usually takes some minutes and is sent out on BSC, exactly to your address - you just have to switch to BSC-network in the wallet.

**If it takes longer than 20 minutes until your bwJUP arrives, you can check on [bscscan](https://bscscan.com/tokentxns?a=0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca&p=1) if your tx was sent.**

**If not, open a support ticket on the [Jupiter homepage](https://gojupiter.tech/support/) and enter some details like your address and the tx-hash for example.**

Thats it, you just swapped your JUP to bwJUP.



## bwJUP to ERC20 JUP

It is pretty much the same as ERC20 JUP to bwJUP, follow the steps there (same addresses, same links, same wallet (yours ;) ).

**Just one important thing**, because of the high tx-fee on ETH-Network, your swap is charged by an amount of JUP (currently 100 JUP, depends on JUP-Price and is adapted, manually i guess). You pay the tx-fee on BSC, which is rather cheap and the charged fee is for the gateway that processes the tx on the ETH-Network.



### One last note

As the BSC-nodes are somewhat unstable, it occurs that a swap stuck on the gateway. No worries, as long as you see your tx incoming on the block explorer of the network you sent it from - if ERC20 JUP [ETH](https://etherscan.io/address/0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca#tokentxns) or bwJUP [BSC](https://bscscan.com/tokentxns?a=0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca&p=1) - your funds are safe. They are logged on the gateway and can be processed manually - therefore open a ticket on [Jupiter homepage](https://gojupiter.tech/support/)