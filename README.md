# Иeureal Wallet
A simple Ethereum Wallet based on Иeureal ERC20 Token. Send a Receive ETH and Иeureal with ease and security. Ethereum wallets are decrypted and raw transactions are signed locally. Raw Transactions are sent directly to EtherScan.io. This application is not an official release from Иeureal, just a opensource wallet for Иeureal Token holders. Wallet Private Keys are kept on your local machine, everytime you want to use this wallet you must re-use the Keystore JSON or Private Key for your wallet.
This wallet is locked to the Иeureal Token contract address: `0x91923993C4Dc3e089BBb1fc9d4A5A765A479B68f`

  <img src="http://i.imgur.com/GEzvKW8.png">

## Иeureal Wallet Features
- Use Keystore JSON wallet
- Use Private Key wallet
- Send and Receive Ethereum (ETH)
- Send a Receive Иeureal tokens. ([0x91923993C4Dc3e089BBb1fc9d4A5A765A479B68f](https://etherscan.io/address/0x91923993C4Dc3e089BBb1fc9d4A5A765A479B68f))
- Set custom Gas Price for transactions
- Portfolio value for Иeureal and Ethereum in USD
- Copy address to clipboard when clicked
- Transaction ID with etherscan URL once transaction is submitted
- Check for Updates button (in About - bottom right)
- Raw Transactions send to EtherScan

<img align="left" width="520" src="http://i.imgur.com/abtoXeH.png"><h3>Wallet Security</h3>
None of your wallet information is sent to any server. This wallet uses [ether-js](https://docs.ethers.io/ethers.js/index.html) javascript library to decrypt wallets locally. Each time you open the wallet, you will need to reinput the Keystore JSON file with password or use the wallet's Private Key. To keep your wallet secure, I highly recommend using the Keystore JSON at all times. To remove confusion, this wallet will not allow you to create a new wallet. If you don't have a Ethereum or Иeureal wallet yet, make one with a secure password at [myetherwallet.com](https://www.myetherwallet.com/). This wallet will not save or move your wallets. Be sure to back up the Keystore JSON file!

<h3>Transactions</h3>
This Иeureal Wallet will allow you to set a custom Gas Price if you need to change the price. By default it is set to *21* gwei. Minimum is 5 gwei. The gas limit on a normal Ether transaction is *12000*. The gas limit on sending Иeureal Tokens is *65000*.

<img align="right" width="420" src="http://i.imgur.com/GiwYFi5.png">

<img align="left" width="420" src="http://i.imgur.com/zo6VaGE.png">


<h3>Source Code Auditing</h3>
Feel free to look at what this application is doing. Иeureal Wallet was built in electron, jquery, bootstrap, and uses ether.js for decrypting wallets. Below you'll find the main functionality of the application.

### Audit Lines
- [ИeurealToken Contract](https://github.com/hunterlong/neureal-wallet/blob/master/js/main.js#L22)
- [Send Ethereum Transaction](https://github.com/hunterlong/neureal-wallet/blob/master/js/main.js#L319)
- [Send Иeureal Transaction](https://github.com/hunterlong/neureal-wallet/blob/master/js/main.js#L367)
- [Decrypting Keystore JSON](https://github.com/hunterlong/neureal-wallet/blob/master/js/main.js#L276)
- [Using Private Key](https://github.com/hunterlong/neureal-wallet/blob/master/js/main.js#L163)

### Build
You can compile this electron application on your own.
- `git clone https://github.com/hunterlong/neureal-wallet`
- `cd neureal-wallet`
- `npm install`
- `npm start`

# License
This wallet is for the Иeureal community to make life 2% easier for us ERC20 token holders. If you have any fixes or updates, please submit a PR. That'd be awesome! This wallet was NOT created by Neureal, so take this as unofficial but useable. Source code is MIT, make your Иeureal ERC20 Token experience decentralized!

### Donate :beer::bug:
ETH/NECP: `0x41FB95D55fB0B353A82814a876Cd0BEea2b29337`
