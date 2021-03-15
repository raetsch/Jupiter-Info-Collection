# Fundamentals of JUP and some explanations

JUP has maximum supply of **1.000.000.000** Coins. It is a modified NXT-source and so, if someone is talking about native JUP, he talks about this.



However, currently JUP exists on 3 Chains and to lower confusion a bit, i try to shed some light on that:

- JUP as ERC20 - correct name would be wJUP, but that was a mistake on creation so it is also named JUP (look at the pair on uniswap https://info.uniswap.org/pair/0x2dfee82f4250dd3f3c6811c5d2926ede8b37a7d5). Also **1.000.000.000** (w)JUP on ERC20 exist. 
  At the beginning the native JUP was swapped to ERC20-JUP via a manual "gateway" (Currently only native to bsc is active due to the fees on ETH-Network). Here is the JUP-gateway-address: JUP-V5K2-269Z-QHGN-FSFT8. It currently (March 14th, 2021) holds 283.172.086 JUP. 

  The ERC20-side of the gateway currently holds 144,340,165 JUP on address [0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca](https://jupitertoolkit.com/explorer/address/0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca)

- bwJUP as bep20 (on BSC) - binance wrapped JUP. The contract address is 0x0231f91e02DebD20345Ae8AB7D71A41f8E140cE7 and also supply is **1.000.000.000**.

  Currently swaps from native JUP are only possible to bwJUP. This is still done manual but will be automated in the future. The native JUP-address is also JUP-V5K2-269Z-QHGN-FSFT8 and the same goes for the bsc-address of the gateway [0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca](https://bscscan.com/address/0x34fbbb37eb4f50f447e736e7b771bd3ad20c41ca#tokentxns)

  

