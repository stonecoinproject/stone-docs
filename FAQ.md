FAQ
========================

## GENERAL

#### Where can I buy STONE?

- CryptoBridge: https://wallet.crypto-bridge.org/market/BRIDGE.STONE_BRIDGE.BTC
- Crex24 Exchange: https://crex24.com/exchange/STONE-BTC

#### I found a bug what should I do?

- Log into [STONE Discord](https://discord.gg/7ZuCMmz) and report it in [#bugs](https://discord.gg/7ZuCMmz), thank you to help us improving STONE.

#### How can I invite people to STONE's Discord?

- This is the invitation link to STONE Discord: https://discord.gg/QaXXEaa

#### Can I support STONE Project?

- Yes! The Stone Project is built by the community and for the community. Anyone who is interested in supporting STONE can get in touch with the Core Team Members. All skills and backgrounds are welcome. All members contribute on a volunteer basis at this time.

## WALLET

#### Where do I find the newest wallet version?

- The newest versions of the wallet (Windows, Linux & Mac) are available at https://github.com/stonecoinproject/Stonecoin/releases

#### How can I update my local wallet?

- Make a backup of your wallet.dat, Masternode.conf, Stonecoin.conf, delete your blocks and chainstate folders, then run the new wallet. You can also go to options and reindex.

#### How do I update my VPS wallet

Simply run the script below and select Option 2

```
wget -O - https://raw.githubusercontent.com/stonecoinproject/stonemnsetup/master/stonemnsetup.sh | bash
```

#### Where do I find my local STOE wallet?

Config file locations for Windows and Mac OS are in

- Windows: %APPDATA%\StoneCrypto\
- Mac OS: ~/Library/Application Support/StoneCrypto/ Unix/Linux: ~/.stonecrypto/

Note: Make sure that your [Library is visible](https://knowledge.autodesk.com/support/fusion-360/troubleshooting/caas/sfdcarticles/sfdcarticles/How-to-Access-Hidden-User-Library-folder-on-Mac-OS.html).

#### Where do I find my config files for the STONE wallet?

- In the navigation menu click on Tools and you will be able to open your .conf files


## MASTERNODE

#### I have problems setting up my Masternode

- Did you run the installation script below and followed its steps?

```
wget -O - https://raw.githubusercontent.com/stonecoinproject/stonemnsetup/master/stonemnsetup.sh | bash
```

If you still have problems join STONE Discord and ask for help in [#hellllllpppp](https://discord.gg/DPfR9ge)!

How many STONE do I need for a Masternode?

- You need 1500 STONE as collateral.

How do I setup a Masternode?

- You will find the setup guide here #guides

How do I update my Masternode?

- You will find the updated guide here #guides

What do I do if my masternode reads "new restart required"?

1. Close local wallet, delete "mncache.dat" in your %appdata%/StoneCrypto dir, restart wallet. If that did not work go on to step 2.
2. Go to VPS and type:

```
rm -r ~/.stonecrypto/blocks ~/.stonecrypto/chainstate
stonecoin-cli stop
```

3. If you used the Stonecoin MN Setup script then let sync (if not, run "stonecoind -daemon"), open the local wallet and press "start alias"

My VPS wallet did stop syncing

- If your VPS has stopped and needs to be resynced, below there are simple two steps to help you resync your masternode:

```
rm -r ~/.stonecrypto/blocks ~/.stonecrypto/chainstate
stonecoin-cli stop
```
