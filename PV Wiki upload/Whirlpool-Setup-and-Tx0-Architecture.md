Please see the Samourai Wallet [Whirlpool Github](https://github.com/Samourai-Wallet/Whirlpool) for a more in depth analysis.

## Table of Contents
* [**1. CLI Setup**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Whirlpool-Setup-and-Tx0-Architecture#1-whirlpool-cli-setup-and-run)
* [**2. GUI Setup**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Whirlpool-Setup-and-Tx0-Architecture#2-whirlpool-gui-setup-and-run)
* [**3. Tx0 Process**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Whirlpool-Setup-and-Tx0-Architecture#3-tx0-and-the-process)
* [**4. Other Whirlpool Links**](https://github.com/PuraVlda/samourai-wallet-android/wiki/Whirlpool-Setup-and-Tx0-Architecture#4-other-whirlpool-links)

### 1. Whirlpool CLI Setup and Run

1. Go to [Whirlpool Releases](https://github.com/Samourai-Wallet/whirlpool-client-cli/releases)
2. Download latest CLI version and put in designated folder you want to run the program from
3. Make sure you have Java 8+ (JDK) downloaded and installed on your device (get [here](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html))
     * Check by opening Terminal/Command Line and type `java --version`
4. Open Terminal and cd (Change Directory) to where you put the CLI (.jar) file
5. Execute `java -jar **<name_of_current_whirlpool_client_file>**.jar --init` to initialize the CLI and wallet.  Here you will be prompted to upload your Whirlpool Payload text blob from your Samourai Mobile Wallet.  
6. Once `--init` is executed you will be prompted to restart CLI.
7. With the CLI there are multiple commands you can provide which will tell Whirlpool what to do, some examples below:
     * `java -jar **<name_of_current_whirlpool_client_file>**.jar --server=mainnet --tor --auto-mix --authenticate --debug --debug-client --mixs-target=0` 
     * More Commands:
          * `--init` (initialize the wallet)
          * `--listen` (connect GUI remotely)
          * `--clients=3` (number of clients running i.e. multiple pools)
          * `--client-delay=5` (delay between mixes)
          * `--pool=0.5btc,0.05btc,0.01btc` (priority of pools to mix)
          * `--auto-tx0=0.05btc` (CLI will auto Tx0 any available UTXO's that enter your Deposit wallet)
          * `--proxy=` (socks|http)://host:port
          * `--scode=` (special code provided by Samourai i.e. discounts)
          * `--tx0-max-outputs=` (max output for a Tx0 transaction)
     * Terminate CLI - "killall java"

[CLI Information](https://github.com/Samourai-Wallet/whirlpool-client-cli)

### 2. Whirlpool GUI Setup and Run

1. Go to [Whirlpool Releases](https://github.com/Samourai-Wallet/whirlpool-gui/releases)
2. Download latest Whirlpool GUI version and install on your device
3. Make sure you have Java 8+ (JDK) downloaded and installed on your device (get [here](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html))
     * Check by opening Terminal/Command Line and type `java --version`
4. Run Program and follow prompts

[GUI Information](https://github.com/Samourai-Wallet/whirlpool-gui)


### 3. Tx0 and the Process

* Merging UTXO’s Prior to Tx0 - See explanation of [Merging](https://github.com/PuraVlda/samourai-wallet-android/wiki/Bitcoin-Privacy-Best-Practices) on the Best Practices Page.

* Premix UTXO's, Fees, Change and OP_Return

     * Premix UTXO's - Equal sized UTXO's will enter Premix based on pool size.
     * Fees - There are Samourai Fees and Miner Fees
          * Samourai Fee - 5% of the Pool Size paid once with unlimited Mixing (Pool sizes are .01, .05 and .5) 
          * Miner Fee - There is a miner fee to compose the initial Tx0 Transaction and there will also be a small miner fee attached to each Premix UTXO.  For a mix to start there are 3 Premixers (up to 4) and 2 Postmixers (down to 1).  Premixers will pay the mining fee for the mix and the Postmixers are considered "Freeriders".
     * Change - Remaining Bitcoin not able to be mixed.  This is separated and kept in account 0.
     * OP_Return - Used to convey data to the coordinator such as codes info


### 4. Other Whirlpool Links

* Read the TLDR on Github - https://github.com/Samourai-Wallet/Whirlpool
* Guides for using Whirlpool Deskop - https://support.samourai.io/section/38-whirlpool
* Video Playlist - https://www.youtube.com/watch?v=0FiIGhi3_R0&list=PLIBmWVGQhizIWHyDkY-AzYc-Rn_3zGRct
* Latest GUI binaries (all platforms) - https://github.com/Samourai-Wallet/whirlpool-gui/releases/latest
* Java required on your desktop pc - https://m.wikihow.com/Check-Your-Java-Version-in-the-Windows-Command-Line
* **More from the Samourai Team** - [Understanding Pools and Fees](https://support.samourai.io/article/81-understanding-pools-and-pool-fees)
* **General Whirlpool Overview by @6102bitcoin** - [Overview](https://github.com/6102bitcoin/FAQ/blob/master/whirlpool.md)
* How to use Whirlpool translated in Spanish [here](https://medium.com/@Multicripto/c%C3%B3mo-hacer-coinjoin-en-whirlpool-con-samourai-wallet-bc5b599f87b8) by @Multicripto

