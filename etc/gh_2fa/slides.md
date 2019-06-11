---
title: 2FA and Signing with GitHub
author: By Christian "chrissx" Häußler
theme: Copenhagen
---

# Previously on chrissxYT/i3buntu
* ghk/ghp
* no signing

# ghk & ghp
```sh
echo "key" | openssl aes-256-cbc -a -in - -out ~/.ghk.enc
```
## ghk
```sh
openssl aes-256-cbc -d -a -in ~/.ghk.enc -out -
```
## ghp
```sh
ghk
git push
```
## problems
* copy-pasting is annoying
* the key is visible on your screen -> bad idea at conferences, etc
* you have to re-enter your passphrase every time

## why i used them
* i cant pipe creds into git push
* you have to code a cred helper, wtf is that?!

