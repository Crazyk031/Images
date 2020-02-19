Samourai Wallet has the most comprehensive package of Post Mix Spending Tools available today.  People underestimate the importance of Post Mix transactions and they are as important if not more important than the Coin Join Mix itself.

## Table of Contents
* [**1. Importance of Post mix**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Post-Mix-Tools#1-importance-of-post-mix)
* [**2. Stonewall**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Post-Mix-Tools#2-stonewall)
* [**3. Stonewallx2**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Post-Mix-Tools#3-stonewallx2)
* [**4. Stowaway**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Post-Mix-Tools#4-stowaway)



### 1. Importance of Post Mix

[Anon-set is a flawed metric](https://medium.com/samourai-wallet/diving-head-first-into-whirlpool-anonymity-sets-4156a54b0bc7?sk=f47e1883c931071c849635c0c797a7c1)
* Anon-set degradation matters
* Beware Timing / Fee rate analysis when sending to cold storage
* Remixing is essential but not encouraged by design except within Whirlpool


### 2. Stonewall 
Stonewall is a Mini Coin Join which hides paid amount.
* Aim to make every Post Mix Spend at least a Stonewall.

[Website](https://samouraiwallet.com/stonewall)

[Stonewall Transaction Setup](https://gist.github.com/SamouraiDev/4ced85a29996dd56781e2bf319b93aaf)


### 3. Stonewallx2 
A Stonewallx2 creates a mini Coin Join using a friend's UTXO set.
* Hides actual paid amount  
* You can spend this Transaction to any wallet.
* Since you cannot distinguish STONEWALL from STONEWALLx2, doubt is created for all transactions that may be observed as a STONEWALL by blockchain observers as to the number of true participants (1 or 2). This is how you defeat CA – by breaking their assumptions and heuristics.


[Stonewall Thread](https://mamot.fr/@laurentmt/101411217125803868)


### 4. Stowaway  
A Stowaway creates a PayJoin using a friend's UTXO set.  
* This is a Payjoin and does not appear so on blockchain.  This transaction is made to be sent to another Samourai Wallet user.

[Website](https://samouraiwallet.com/stowaway)
