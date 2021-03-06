# Nsign
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/tarithj/nsign)
![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/tarithj/nsign/latest)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/87bfd651a5764815acd1839132fc8c7f)](https://www.codacy.com/manual/tarithj/nsign/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=tarithj/nsign&amp;utm_campaign=Badge_Grade)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript Style Guide](https://img.shields.io/badge/code%20style-google-blueviolet.svg)](https://github.com/google/gts)   
A super fast user-friendly file signing and verification software   
![nsign](https://upload.wikimedia.org/wikipedia/commons/5/54/Screenshot_of_nSign_v1.1.0.png)

## What is Nsign(NanoSign)
Nsign is a file signing and verification software.

### Why?
It's hard to verify if the file received from the internet is by the actual creator or an impersonator. 
This is the main reason nsign was made; To create a new way of online identification.

### Uses
* Online identification (example: To verify if a software is created by the official developers)
* Approval

## Q&A
**Q - How dose this work**   
A - Nsign works by using public-key cryptography ([learn more](https://en.wikipedia.org/wiki/Public-key_cryptography))

**Q - Does nsign require internet**   
A - Nsign works fully offline, No internet connection needed.

**Q - What happens if I lose my private key**   
A - If you lose your private key you should generate a new key-pair and send the public key to the other people who used your old public key to verify you.

**Q - What happens if I forget my private key password**   
A - When you generate your key-pair with a password nsign encrypts the private key with the password to keep it safe but if you forget the password you won't be able to sign with that private key and the private key will be considered lost. The only option is to create a new key-pair.

**Q - What happens if Someone stole my private key**   
A - You should quickly generate a new key-pair and send the new public key to the people who used your old public key and tell them to only trust your new key.

## Getting started
1. Download the latest release from [here](https://github.com/tarithj/nsign/releases/latest)
2. Start nsign
3. Select generateKey
4. Follow the instructions

### Signing
1. Start nsign
2. Select sign
3. Enter the password that was asked when you first generated the keys
4. Enter the location of the private key (example: ./privateKey_256.nSignE)
5. Enter the location of the file you want to sign (example: ./test.pdf)

### Verifying
1. Start nsign
2. Select verify
3. Enter the location of the public key (example: ./publicKey_256.nSign)
4. Enter the location of the file you want to verify (NOTE: The .nSignSig file must be in the same location as the file. Example: ./test.pdf)

