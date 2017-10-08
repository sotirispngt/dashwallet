![header](/images/mueheader.jpg)

muewallet (breadwallet fork) is a real standalone mue client. There is no server to get hacked or go down, so you can always access your money.
Using [SPV](https://en.bitcoin.it/wiki/Thin_Client_Security#Header-Only_Clients) mode, muewallet connects directly to the mue network with the fast performance you need on a mobile device.

muewallet is designed to protect you from malware, browser security holes, even physical theft. With AES hardware encryption, app sandboxing,
keychain and code signatures, muewallet represents a significant security advantage over web and desktop wallets, and other mobile platforms.
Simplicity is muewallet’s core design principle. A simple backup phrase is all you need to restore your wallet on another device if yours is ever lost or broken.
Because muewallet is [deterministic](https://muepay.atlassian.net/wiki/display/DOC/Whitepaper), your balance and transaction history can be recovered from just your backup phrase.

#####Features:
- [“simplified payment verification”](https://muepay.atlassian.net/wiki/display/DOC/Official+Documentation) for fast mobile performance
- no server to get hacked or go down
- single backup phrase that works forever
- private keys never leave your device
- import [password protected](https://muepay.atlassian.net/wiki/display/DOC/Official+Documentation) paper wallets
- [“payment protocol”](https://muepay.atlassian.net/wiki/display/DOC/Official+Documentation) payee identity certification
- Shapeshift integration (Pay any BTC Address by just scanning the BTC QR Code)

#####URL scheme:
muewallet supports the [x-callback-url](http://x-callback-url.com/) specification with the following URLs:
```
mue://x-callback-url/address?x-success=myscheme://myaction
```
this will callback with the current wallet receive address: myscheme://myaction?address=1XXXX
the following will ask the user to authorize copying a list of their wallet addresses to the clipboard before calling back:
```
mue://x-callback-url/addresslist?x-success=myscheme://myaction
```

![footer](/images/muefooter.jpg)

#####WARNING:

installation on jailbroken devices is strongly discouraged

Any jailbreak app can grant itself access to every other app's keychain data
and rob you by self-signing as described [here](http://www.saurik.com/id/8)
and including `<key>application-identifier</key><string>*</string>` in its
.entitlements file.

#####INSTALLATION:

[Download Install Guide](https://muepay.atlassian.net/wiki/display/DOC/Download+-+Install+-+Guide)
