# Ledger App Installer

### Description
Browser installer for Ledger hardware wallet apps. This provides an easy way to distribute your app outside of Ledger Live.

### How To Use
Download or fork this repo and apply the following changes to the [apps.js](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/apps.js) file to make this installer install your app.
1. [Change the firmware version](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/apps.js#L11) to the [SDK version](https://github.com/LedgerHQ/nanos-secure-sdk/blob/master/include/bolos_version.h#L2) that you used to build your app.
2. [Change the app name](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/apps.js#L31) to your app's name.
3. [Change the app version](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/apps.js#L34) to your app's version.
4. [Change the hash](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/apps.js#L40) to your app's hash. This can be found in the bin/app.sha256 file that's created when you built your app.
5. [Change the APDU commands](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/apps.js#L50-L234) to your app's APDU commands. This can be found in the bin/app.apdu file that's created when you built your app.

After those changes are performed, you can open the [index.html](https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/index.html) in a [web browser that supports WebUSB](https://caniuse.com/webusb) and use it to install your app onto a Ledger hardware wallet.

If you fork this repo, you can use [GitHub's HTML Preview](https://htmlpreview.github.io/) feature to install your app without having to download and open the index.html file. To do so, change this link [https://htmlpreview.github.io/?https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/index.html](https://htmlpreview.github.io/?https://github.com/NicolasFlamel1/Ledger-App-Installer/blob/master/index.html) to point to your repo and visit that link.
