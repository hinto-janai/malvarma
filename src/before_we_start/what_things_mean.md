# What things mean
This guide can be used without reading this page, skip if desired.

---

Following this guide may be easier if you have basic knowledge of some things.

The following are simplified explanations of some important concepts related to cold wallets.

## 🌪 Air-gapped
An [air-gapped](https://en.wikipedia.org/wiki/Air_gap_(networking)) device is a device that is isolated from any conventional network (internet, LAN, etc) via software and/or physical means.

Note that, while an air-gapped device is incapable of networking, it is still capable of 2-way data transfer via USB, SD Card, etc.

Hardware wallets such as the [Trezor One](https://trezor.io/trezor-model-one) do not have any software capabilities nor any [physical circuitry](https://github.com/trezor/trezor-hardware/blob/master/electronics/trezor_one/trezor_v1.1.sch.png) that allow for network interfacing, thus it could be considered an air-gapped device. All data transfers (including firmware changes) occur via USB.

Similarly, a computer lacking the physical hardware to network (WiFi/Bluetooth chip and/or Ethernet port) would also be considered air-gapped.

"Cold" is usually used as a synonym for air-gapped.

## ❄️🔥 Cold/Hot wallet
A `cold` wallet is a wallet that employs the air-gapped techniques described above and is not connected to any network.

A `hot` wallet is a wallet that _is_ connected to a network in some form or another.

## ✒️ Signing a transaction
When you send Monero, you are authorizing a transaction with your **private spend key**.

Like a check:
- You see **who** it is going to
- You see **how much** money is being sent

All that is left is for you (your wallet) to authorize the transaction by "signing" it.

Just like a check with a name and amount, a transaction can be created relatively easily - but without your signature it is not a "real" transaction.

## 🔑 Spend/View key
Monero wallets are made up of 4 keys:
- Private spend key
- Private view key
- Public spend key
- Public view key

What each of these are used for is not too important for the purposes of this guide.

The important thing to take away is that the **private spend key** is the only key that can spend funds.

When you create a "view-only" wallet in Monero, it is a wallet that has access to all keys **except the private spend key**, thus it cannot spend funds (but it can see incoming funds just fine).

## 💽 Key Images & Outputs
Again, what these things are is not too important for the purposes of this guide.

The important thing to take away is that the these two things (key images & outputs) are additional pieces of data that must be carried over from `cold <-> view` wallets in order for:
- The `cold` wallet to see an updated balance
- The `view` wallet to see outgoing funds
