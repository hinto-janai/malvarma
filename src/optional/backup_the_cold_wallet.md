# Backup the cold wallet
Following this guide, your cold wallet only exists on a single, physical machine.

This is risky - if that machine were to to fail, your cold wallet would be gone with it.

---

It is encouraged to backup your cold wallet in some type of way, whether this means saving your seed, or the file itself.

The many ways to do this are outside the scope of this guide, but they can easily be found by searching around.

**Your seed/cold wallet should never leave your air-gapped device unencrypted**.

Use [well-known](https://www.gnupg.org) and [trusted](https://www.veracrypt.fr) encryption software to encrypt your wallet before transferring it to a machine connected to the internet or any other network. Even Monero wallets themselves have built-in password and encryption schemes, use them if needed.
