# ⛔️ Before we start

<p style="background:rgba(200,250,155,0.2);padding:0.75em;">
<strong>This guide is meant to be read from front-to-back, in order.
<br>
<br>
There are steps that may not be applicable to you, if so, feel free to skip them.
</strong>
</p>

---

At the end of this guide, you will be in possession of an [air-gapped](https://en.wikipedia.org/wiki/Air_gap_(networking)) device.

For the purposes of this guide, we focus on how to use that device to create and sign offline Monero transactions, however, there are other practical usecases this device could serve, e.g:

- Other offline cryptocurrency transaction signing
- Offline password vault ([KeePassXC](https://keepassxc.org), [Bitwarden](https://bitwarden.com), [1Password](https://1password.com), etc)
- Offline [OTP/2FA](https://en.wikipedia.org/wiki/Multi-factor_authentication) generation
- Offline PGP message signing

In short, this air-gapped device is viable for storing any "secret" that would be better stored offline, and is not just limited to Monero.
