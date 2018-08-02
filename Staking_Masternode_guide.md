![logo](https://aquila.online/images/logo2x.png)

## Requirements

### Staking
  * No Minimum amount of coins to stake. *(The more, the better though)*
  * The AQX coins you intent to stake must have 60 confirmations.
  * Synchronized [AQX wallet.](https://github.com/aquilacoin/Wallets)
  * Dedicated machine for your wallet, as you want to keep it online as much as possible.
  
### Masternode
  * Exactly 5000.00 AQX as collateral. *(Send 5001+ to wallet from exchange to cover fees)*
  * Dedicated Linux (Ubuntu 16.04) VPS from [Vultr.](https://www.vultr.com/?ref=7454181) 
    * *$5 Vultr server will do. (Can safely run Approx. 3-4 different coins)*
  * Synchronized [AQX wallet.](https://github.com/aquilacoin/Wallets)
-----
### Setting up for Masternode & Installing VPS
  * Assuming that you have transfered coins from exchange to wallet. *(5001+ to cover transaction fees)*
    * Create a new reciving address - File - Recivievg address - New - Name new address MN1.
    * Send 5000 exactly to MN1.
    * Wait for 1 confirmation on transaction.
    * Goto Tools - Debug Consol.
    * Type masternode outputs. *(Copy and save for later)*

 * Now logon to your VPS via Putty or prefrable choice.  

 * Download the install script.
```    
wget -q https://raw.githubusercontent.com/turbowrx03/Guides/master/VPS%20Install/AQX_Install.sh

```
-----    
  * Run the script and input the proper information during the prompts.
```
chmod u+x AQX_Install.sh
./AQX_Install.sh

```
-----
* Start Aquila.
```
./Aquilad -daemon

```
  * If you get a message asking to rebuild the database, please hit Ctr + C and run ./Aquilad -daemon -reindex
