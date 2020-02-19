## Table of Contents
* [**1. General**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions#1-General)
* [**2. Dojo**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions#2-dojo)
* [**3. Mobile Wallet**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions#3-mobile-wallet)
* [**4. Post Mix Tools**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions#4-post-mix-tools)
* [**5. Sentinel**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions#5-sentinel)
* [**6. Whirlpool**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions#6-whirlpool)

### 1. General

   * Q: **Is Samourai Wallet Open Source?**
   * A: Yes, Samourai Wallet is open source.  All source code for all Samourai Wallet projects can be found at the Samourai Wallet [GitHub Page](https://github.com/Samourai-Wallet)

------------------------------------------------------------------------------------------------------------------
   * Q: **Is Samourai Wallet Private?**
   * A: Samourai Wallet has many tools and features that allow users to make transactions with improved on-chain privacy. By default Samourai Wallet connects to the Samourai server to monitor address balances so users should consider running their own backend (DOJO) to be a self sovereign user with maximum privacy. This can be done easily using either a [DIY](https://github.com/PuraVlda/samourai-wallet-android/wiki/Dojo-Node) node or buy a [Samourai nodl](https://shop.nodl.it/en/home/38-nodl-samourai-edition.html).

------------------------------------------------------------------------------------------------------------------
   * Q: **Where can I find general Samourai Wallet Support Docs?**
   * A: Samourai Wallet support docs can be found [here](https://support.samourai.io/)

------------------------------------------------------------------------------------------------------------------
   * Q: **What BIPs does Samourai Wallet support ?**
   * A: You can find the list of supported [BIPs](https://samouraiwallet.com/bips) here

------------------------------------------------------------------------------------------------------------------

   * Q: **Where do I get badass Samourai Wallet Merch?**
   * A: There are 2 places right now;
     * [Lightning Hood](https://lightninghood.com/shop): Shirts, hats and other accessories
     * [nodl Samourai Edition](https://shop.nodl.it/en/home/38-nodl-samourai-edition.html): Samourai Edition nodl Full Node and Dojo device

------------------------------------------------------------------------------------------------------------------

   * Q: **Will Samourai Wallet provide any information to State or Government actors if required?**
   * A: The goal of Samourai Wallet is to create the most private bitcoin wallet and feel that compliance with certain laws will create a material negative for our users. On the Samourai Wallet Website they have provided a [Warrant Canary](https://samouraiwallet.com/canary) which is renewed every 365 days. If this does not show renewed on the date stipulated, you should assume the worst.

------------------------------------------------------------------------------------------------------------------
   * Q: **Is Samurai Wallet available on Desktop?**
   * A: No, Samourai Wallet is a mobile only wallet. There is a Whirlpool Desktop App for Coin Join but it is not a full wallet.

------------------------------------------------------------------------------------------------------------------
   * Q: **Is the Samourai Wallet wiki translated into other languages?**
   * A: Yes, community members are helping with this as we speak.  Below are what is available and will be updated:
     * Samourai wiki in Spanish [here](https://github.com/4rkad/samourai-wallet-android/wiki)

          
------------------------------------------------------------------------------------------------------------------
### 2. Dojo

 * Q: **What are my options for building a Dojo?**
 * A: You can buy a Pre-built Dojo node or use the open source software from Samourai to build yourself with various hardware.  See [Dojo](https://github.com/PuraVlda/samourai-wallet-android/wiki/Dojo-Node) page for more information.
------------------------------------------------------------------------------------------------------------------
 * Q: **If Dojo doesn't seem to be working right where do I go to check?**
 * A: Dojo is pretty much a self reliant piece of software, if it is not acting right most likely the logs will tell you.  To run these logs you must Open Command, Terminal (Mac) or PowerShell (WIndows) and Change Directories (cd) to where your dojo.sh script is; i.e. `Documents>dojo_dir>docker>my-dojo`.  Once there, you can run the following commands to open up logs:
     * `./dojo.sh logs` - display the logs of all containers
     * `./dojo.sh logs bitcoind` - display the logs of bitcoind
     * `./dojo.sh logs db` - display the logs of the MySQL database
     * `./dojo.sh logs tor` - display the logs of tor
     * `./dojo.sh logs api` - display the logs of the REST API (nodejs)
     * `./dojo.sh logs tracker` - display the logs of the Tracker (nodejs)
     * `./dojo.sh logs pushtx` - display the logs of the pushTx API (nodejs)
     * `./dojo.sh logs pushtx` -orchest - display the logs of the Orchestrator (nodejs)
------------------------------------------------------------------------------------------------------------------
 * Q: **How do I check errors in the various Dojo logs?**
 * A: By using one of the commands from the question above you can add the following to the end `-d error -n 500` 
i.e. `./dojo.sh logs tracker -d error -n 500`
------------------------------------------------------------------------------------------------------------------

### 3. Mobile Wallet

   * Q: **What are all the features on Samourai Wallet?**
   * A: There are too many features to list but there is a nice compilation [here](https://github.com/Samourai-Wallet/samourai-wallet-android/blob/develop/Samourai-Wallet-features.md)
------------------------------------------------------------------------------------------------------------------
   * Q: **When is Samourai Wallet coming to iOS?**
   * A: "Very difficult to find experienced iOS who understand Bitcoin, who are willing to work like the rest of us (for passion not profit right now) and who are reliable enough to stick around. It's been a challenge . Sentinel iOS will be out soon. But many things need to be written from scratch. Every iOS wallet is just a javascript bridge. To us that is not acceptable. So i will be released when it is ready, and not a day before." - SW
------------------------------------------------------------------------------------------------------------------
   * Q: **Is Samourai Wallet compatible with Hardware Wallets**
   * A: Right now Samourai Wallet is not compatible with other Hardware wallets, although, it is compatible with [Opendime](https://opendime.com/).  You can find more information on Opendime compatibility [here](https://samouraiwallet.com/opendime).  There may be future integration of Partially Signed Bitcoin Transactions (PSBT) coming up.
------------------------------------------------------------------------------------------------------------------
   * Q: **What do I do if I need Support Help?**
   * A: Email support@samouraiwallet.com if possible, they'll be able to help you more and take a look at your particular situation.  To make things faster you can include a support backup in your email to support. you can find this in `settings >troubleshooting>send support backup`
------------------------------------------------------------------------------------------------------------------

   * Q: **What is the best practice for backing up your seed on Samourai Wallet?**
   * A: There are many options to back up seed phrases for all wallets out there.  These are some guidelines we go by:
     * When backing up your seed phrase you should use offline solutions like writing it down or a [cryptosteel](https://cryptosteel.com/shop/)
     * Do not take a screenshot! Do not email it to yourself. Write it down and treat it like the precious document it is
     * Take it up a notch and get a [cryptosteel](https://cryptosteel.com/shop/) if you're worried about fire damage, or the long term viability of your piece of paper

> The app space on android is totally separate from any other app, isolated. (unless you are running as root on a custom rom, don't do that)
------------------------------------------------------------------------------------------------------------------

   * Q: **What the heck is a PayNym?**
   * A: PayNym is what Samourai Wallet calls it, in reality they are payment codes (BIP47) which are great for privacy. They act very similar to a Private Payment Channel (similar to Lightning Channel) but reside on the blockchain. Imagine you share an address with public and nobody can lookup the balance of it from the blockchain, you don't have to imagine you can start to use them today.  
------------------------------------------------------------------------------------------------------------------

   * Q: **What is Ricochet and does it improve my privacy?**
   * A: Ricochet does not improve your privacy.  Exchanges can sometimes blacklist or "freeze" your bitcoins when they see a Coin Join in your transactions history, ricochet aims to solve these problems by putting distance between you and your exchange by adding hops to your transaction. There is also staggered ricochet which leaves better fingerprint and looks more realistic in the blockchain (it takes longer than the normal ricochet). It is advised to use ricochet when you send bitcoin to your exchange. 
------------------------------------------------------------------------------------------------------------------
   * Q: **How do I restore my Samourai Wallet in Electrum?**
   * A: Please see steps below:
     * Download Electrum [here](https://electrum.org/#download) and don't use any version before 3.3.4
     * Open Electrum and provide a name for your Electrum wallet
     * Select Standard Wallet
     * Select 'I already have a seed'
     * Click 'Options'
     * Check both 'Extend this seed with custom words' and 'BIP39 seed' (Ignore BIP39 warning)
     * Enter your 12-word mnemonic
     * Enter your BIP39 passphrase on the 'Seed extension' screen
     * Type of addresses: 'native segwit (p2wpkh)'
     * Provide a password. You will need this password to open your wallet whenever you use Electrum.
          
------------------------------------------------------------------------------------------------------------------
   * Q: **Can Samurai Wallet be used with Testnet?**
   * A: Yes, Samourai Wallet can be used on Bitcoin testnet but you must build the wallet from source.  Google Play store App will not give the option.

------------------------------------------------------------------------------------------------------------------
   * Q: **How can I generate multiple receive addresses?**
   * A: In the Samourai ecosystem there are 3 ways to generate multiple addresses:
     * Via Samourai Wallet
          * You can use the address calculator in Samourai Wallet via `settings->troubleshoot`. 
               * Select the type of address you want 
               * Change the index # to generate multiple different addresses 
               * Be sure you don't reuse an address!
          * You can manually create addresses through the receive function.
               * Hit the Plus button on the main screen then click receive 
               * Go in and back twice (this fools the wallet into thinking the address is used) 
               * After the third time it will generate a new address each time you hit receive again
               * This option will not show addresses that have previously received a deposit
     * Via Sentinel
          * You can manually create addresses through the receive function
               * Make sure to set up Sentinel with your PUB keys 
               * Hit the plus button on the main screen then choose deposit 
               * Go in and back twice (this fools the wallet into thinking the address is used)
               * After the third time it will generate a new address each time 
               * This can be used for more than just Samourai Wallet

------------------------------------------------------------------------------------------------------------------
### 4. Post Mix Tools

   * Q: **You talk about post-mix and #cahoots what are those ?**
   * A: After doing Coin Join transactions its important to not merge non Coin Joined Bitcoins with Coin Joined ones, that's where #cahoots will help. #Cahoots is the general name of the available post-mix methods that Samourai Wallet has.
------------------------------------------------------------------------------------------------------------------

   * Q: **What are those post-mix methods ?**
   * A: There are 3 methods;
     * Stonewall: A basic transactions that looks like a mini Coin Join in the blockchain
     * Stonewallx2: A real mini Coin Join where your friend provides you inputs
     * Stowaway: A special transaction which looks like a normal transaction but actually is a mini Coin Join between you and your friend where the real transacted amount is obfuscated in the blockchain 
     * [More Cahoots Information](https://github.com/PuraVlda/samourai-wallet-android/wiki/Post-Mix-Tools)
------------------------------------------------------------------------------------------------------------------

### 5. Sentinel

   * Q: **What is the difference between Samourai Wallet and Sentinel ?**
   * A: Sentinel is a watch only Bitcoin wallet tracker for both Android and iOS. You will provide Sentinel with your XPub, YPub and/or ZPub to link your wallet.  With Sentinel you are able to deposit to any wallet you have linked. 

------------------------------------------------------------------------------------------------------------------
   * Q: **Can Sentinel broadcast a Bitcoin Transaction**
   * A: Yes, Sentinel can broadcast a Partially Signed Bitcoin Transaction (PSBT) via QR code or Hex Code.  Sentinel is **NOT** a Bitcoin wallet thus can not **sign** a transaction.

------------------------------------------------------------------------------------------------------------------

### 6. Whirlpool

   * Q: **What is Whirlpool?**
   * A: Whirlpool is the Samourai implementation of Zero-Link Coin Join
------------------------------------------------------------------------------------------------------------------
   * Q: **What is a Coin Join?**
   * A: It's a transaction where people contribute inputs and outputs, it helps to break chain analysis tools, gives you privacy and makes the bitcoin ecosystem more fungible
------------------------------------------------------------------------------------------------------------------

   * Q: **What is the difference in Whirlpool and Wasabi?**
   * A: [Articulated answer by LaurentMT ](https://twitter.com/LaurentMT/status/1187699623386898433)
------------------------------------------------------------------------------------------------------------------

   * Q: **How does Whirlpool work?**
   * A: Whirlpool works by pairing your mobile wallet to the whirlpool desktop GUI/Command Line Client (CLI). There is effectively 4 phases of the mixing process: Deposit, Tx0, Pre-mix, and Post-Mix. The process begins with creating a Tx0. After the Tx0, all the new UTXOs available for mixing get moved into Pre-Mix status. After being mixed with 4 other peers, a new UTXO gets created and is moved to Post-Mix status. 
------------------------------------------------------------------------------------------------------------------
   * Q: **What is a Tx0?**
   * A: A Tx0 is the initial breakdown of your initial UTXO into small equal pieces based on the pool size you joined. What cannot be mixed is sent back to deposit area and is seen in the mobile wallet. So for example if you have one UTXO of 0.1 BTC that you want to mix in the 0.01 pool. You will have 9 new UTXOs that will be queued for mixing. [More info here](https://github.com/PuraVlda/samourai-wallet-android/wiki/Whirlpool-Setup-and-Tx0-Architecture)
------------------------------------------------------------------------------------------------------------------
   * Q: **What is the fee structure of Whirlpool?**
   * A: You pay a one time fee of 5% of the pool. Additionally each new Pre-mix UTXO created requires you pay the miner fee
         * 0.01 pool = 0.0005 BTC + miner fees
         * 0.05 pool = 0.0025 BTC + miner fees
         * 0.5 pool = 0.025 BTC + miner fees 
      * For miner fees, take th example about of 9 newly created Pre-mix UTXOs. You would pay the mixing fee of a one time 0.0005 + mining fees (say 1 sat/b) x 9. 
[More info here](https://github.com/PuraVlda/samourai-wallet-android/wiki/Whirlpool-Setup-and-Tx0-Architecture)
------------------------------------------------------------------------------------------------------------------
   * Q: **Do I have to pay the fees for each mix?**
   * A: No! Once moved into the Post-Mix status, your UTXO is considered a free-rider and will mix for free for every mix after that. This is because the Pre-mixers pay for all miner fees. Hence the term free-rider.
------------------------------------------------------------------------------------------------------------------
   * Q: **How many mixes are enough?**
   * A: This is very subjective. But 1 mix is all that is needed to break the deterministic link from your previous history. However, with every subsequent mix after you privacy increases in significantly. The general guidance is to aim for at least 3, but you can leave your coins mixing until you are ready to spend!
------------------------------------------------------------------------------------------------------------------

   * Q: **What is the difference in a 3-2 and a 4-1 Whirlpool Mix Configuration?**
   * A: A 3-2 mix is referencing to 3 Premix UTXOs and 2 Free ride UTXOs and a 4-1 mix is referencing to 4 Premix UTXOs and 1 Free ride UTXOs.
     * 4-1 guarantees an anon set path to the first mix in  each pool. 5-0 will no longer trigger after the initial mix in a pool.
     * A 4-1 mix may happen if for whatever reason a free rider wasn't reachable for registering. 

> The good thing about Whirlpool is that we can quickly change architecture: pools, denominations, dojo-only, composition of mixes: 3-2, 4-1, 7-3, SCODEs, on the server side with a simple conf file, no dev required. This will allow us to quickly adapt to market conditions while the tx0 architecture shields us from ddos attacks. You should see the number of attempts we get daily for that kind of thing 
------------------------------------------------------------------------------------------------------------------
   * Q: **How do I configure the Whirlpool GUI to work over Tor all the time?**
   * A: If running Dojo, Tor is default and would be running.  If you are not running Dojo, the best way is to make sure Tor is running as a Service in you OS.
     * [OS X Instructions](https://2019.www.torproject.org/docs/tor-doc-osx.html.en) 
     * [Debian/Ubuntu Instructions](https://2019.www.torproject.org/docs/debian.html.en)
     * [Windows Instructions](https://www.torproject.org/download/tor/) 
          * Download Expert Bundle for Windows and follow install guide
          * Install Tor as a Windows Service, simply run the command: `C:\Tor\tor.exe --service install`
------------------------------------------------------------------------------------------------------------------
   * Q: **How can i install and use GUI Whirlpool and use in windows?**
   * A: Please see steps below:
     * Download latest release [here](https://github.com/Samourai-Wallet/whirlpool-gui/releases) 
     * Download and install Samourai Wallet on Android
     * Export Whirlpool Pairing Text Blob and paste into GUI when prompted
     * Video for reference [here](https://www.youtube.com/watch?v=0FiIGhi3_R0&list=PLIBmWVGQhizIWHyDkY-AzYc-Rn_3zGRct)
          
------------------------------------------------------------------------------------------------------------------
   * Q: **How do I restore my Samourai Wallet Post Mix Account in Electrum?**
   * A: Please see steps below:
     * Download Electrum [here](https://electrum.org/#download) and don't use any version before 3.3.4
     * Open Electrum and provide a name for your Electrum wallet
     * Select Standard Wallet
     * Select 'I already have a seed'
     * Click 'Options'
     * Check both 'Extend this seed with custom words' and 'BIP39 seed' (Ignore BIP39 warning)
     * Enter your 12-word mnemonic
     * Enter your BIP39 passphrase on the 'Seed extension' screen
     * Type of addresses: 'native segwit (p2wpkh)'
     * Override suggested derivation path with: m/84'/0'/2147483646' (do not omit trailing ' character)
     * Provide a password. You will need this password to open your wallet whenever you use Electrum.
          
------------------------------------------------------------------------------------------------------------------
   * Q: **How is transaction signing done in Whirlpool CLI/GUI without user input and are funds at risk?**
   * A: Please multiple statements below:
     * No funds are not as risk as you always maintain your Private Keys.  This assumes you practice safe wallet practice.
     * When using CLI/GUI make sure it is used on a trusted device of your own and that good network hygiene is used.
     * When initializing Whirlpool the first time you must import a payload coming from your mobile wallet, this is encrypted information needed to sign such as private keys.  This step is done only once upon Whirlpool initialization.
     * Upon starting Whirlpool your Password decrypts said imported Payload and wallet seed is derived, passphrase is then discarded from use for current run.
     * Address privkeys are derived from seed as needed for signing.
     * Once you close down CLI or GUI you will have to follow the above steps (starting with enter Password) each time you open GUI or run CLI.

          
------------------------------------------------------------------------------------------------------------------
   * Q: **How can I verify my Anon Set within Whirlpool Mixes?**
   * A: Whirlpool mixes are accompanied by verifiable and reproducible anon set values.  You can download the tool to verify yourself [here](https://github.com/Samourai-Wallet/whirlpool_stats).

------------------------------------------------------------------------------------------------------------------

   * Q: **Are Whirlpool instructions translated into other languages?**
   * A: Yes, community members are helping with this as we speak.  Below are what is available and will be updated:
     * How to use Whirlpool in Spanish [here](https://medium.com/@Multicripto/c%C3%B3mo-hacer-coinjoin-en-whirlpool-con-samourai-wallet-bc5b599f87b8)

          
------------------------------------------------------------------------------------------------------------------
   * Q: **What is the difference between a Coin join and Tumbler?**
   * A: Essentially the difference is mathematical.  A Tumbler takes your UTXO's, then mixes them. Coin Join doesn't take your UTXO's, but mixes them with other people's in a way that you never lose control of your UTXO's.  The main and most important difference is that in a CoinJoin you are always in control of your Private Keys.  With a tumbler, you are sending you UTXO's to a third party, they combine into a pool and send you back new UTXO's.  So Coin Joins are the new evolution of tumblers. A Tumbler will, eventually maybe, switch to a Coin Join type mixing. (Or exit scam, their choice).