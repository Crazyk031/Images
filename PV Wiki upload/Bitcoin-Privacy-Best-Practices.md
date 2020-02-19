When it comes to Privacy on the Bitcoin Blockchain there is still some work to do.  Samourai Wallet is making great headway but it will always be a battle to stay ahead of the blockchain snoops.  Below are a list of Best Practices and potential Pitt-falls one must keep an eye out for.

## Table of Contents
* [**1. Block Explorers**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices#1-block-explorers)
* [**2. Information Leaks**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices#2-information-leaks)
* [**3. Key Privacy Heuristics**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices#3-key-privacy-heuristics)
* [**4. Purchase and Sell Bitcoin**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices#4-purchase-and-sell-bitcoin)
* [**5. Sending and Receiving**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices#5-send-and-receive-bitcoin)
* [**6. Other Guides**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices#6-other-guides)

### 1. Block Explorers 

[OXT](oxt.me)

[KYCP](kycp.org)

[Blockstream](blockstream.info)

* The best Explorer setup is one you are running yourself that is referencing back to your own bitcoind for information
* Address look up on external block explorers
     * When looking up information in reference to Bitcoin addresses, Transactions or anything of the sort, make sure you are using at minimum a VPN or Tor.  Make sure between lookups you are switching locations or identities.
* Tor - More information on Tor [here ](https://www.torproject.org/)
     * Switch Identities each search

### 2. Information Leaks 
* What info you dox and to who?

     * Email notifications - Connecting your email to a bitcoin address or Pub Key could potentially harm your Privacy.  It is safe practice to not send this information over email.

     * Screenshots - Crop out your toolbar; leaks much info (apps you run, timezone, networking state, etc...

### 3. Key Privacy Heuristics 

* Coin selection - Use a wallet that gives you full control of your UTXO's.  This will allow you to utilize and benefit from the best Privacy Practices available.
     * When spending make sure to use Post Mix spending tools or select specific UTXO's to spend
     * If you can spend a full UTXO and leave no change that will help with Privacy.  Even if your miner fees need to go up some to achieve this, it is worth the expense.
* Merging UTXO's - Merging UTXO's can drastically degrade your privacy on the blockchain.  If you are not thoroughly paying attention to where each UTXO started and what it was associated with, you could compromise and potentially link UTXO's that were not associated with your identity to ones that were.
     * Separate Wallets - Keep a separate wallet for KYC coins and Non KYC coins
     * Label UTXO's - Label UTXO's to manage potential merging issues in the future

* Labeling UTXO's - Make sure and take advantage of transaction labeling.  This will help you manage UTXO's.

### 4. Purchase and Sell Bitcoin
* Cash Transactions - Cash is King and the best way to purchase Bitcoin anonymously.  Mixing is still encouraged.
* Exchanges - There are both KYC exchanges and Non KYC exchanges.  
     * KYC Exchanges -  Worst for your privacy and Mixing is a must after purchasing.  
     * Non KYC Exchanges - Next best to Cash for purchasing Bitcoin.  Mixing is encouraged after purchase.
          * [Bisq](https://bisq.network/)
          * [hodlhodl](https://www.hodlhodl.com/)
     * Ricochet Tool - Tool from Samourai to put extra hops via Samourai from your wallet and the exchange.
          * [Ricochet Information](https://samouraiwallet.com/ricochet)

[Where to Buy from bitcoin-only](https://bitcoin-only.com/#get-bitcoin)

### 5. Send and Receive Bitcoin

* PayNyms - Public and sharable ID for sending Stealth Payments.
     * [PayNym Information](https://samouraiwallet.com/paynym)
     * [PayNym.is](https://paynym.is/)


### 6. Other Guides

* [hodl-Privacy](https://github.com/6102bitcoin/FAQ/blob/master/hodl-privacy.md) by [ @6102bitcoin](https://twitter.com/6102bitcoin)
* GrapheneOS - A hardened fork of the Android Open Source Project with all Google software stripped out. You can find more information [here ](https://grapheneos.org/)




