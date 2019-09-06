[![version](https://img.shields.io/github/release/Telos-Foundation/Sqrl/all.svg)](https://github.com/Telos-Foundation/Sqrl/releases)
[![issues](https://img.shields.io/github/issues/Telos-Foundation/Sqrl.svg)](https://github.com/Telos-Foundation/Sqrl/issues)
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/Telos-Foundation/Sqrl/master/LICENSE)
![downloads](https://img.shields.io/github/downloads/Telos-Foundation/Sqrl/total.svg)

[English](https://github.com/Telos-Foundation/Sqrl/blob/master/README.md)

[![Sqrl screenshot](https://raw.githubusercontent.com/Telos-Foundation/Sqrl/master/app/renderer/assets/images/sqrl.png)](https://raw.githubusercontent.com/Telos-Foundation/Sqrl/master/app/renderer/assets/images/sqrl.png)

# Sqrl - Telos Full Wallet & Governance dApp

`Sqrl` is a fully functional wallet created by [Telos Miami](https://eos.miami/) for the Telos blockchain that supports any EOS.IO blockchain. This application can be used to connect to a remote EOS.IO API endpoint to securely perform numerous wallet and governance functions.

[![Sqrl screenshot](https://raw.githubusercontent.com/Telos-Foundation/Sqrl/master/Sqrl.png)](https://raw.githubusercontent.com/Telos-Foundation/Sqrl/master/Sqrl.png)

### Features

**NEW FEATURES**:
- **(T-)REX**: Sqrl allows you to participate in the Resource Exchange system, or REX, for any blockchain that supports it. REX allows you to lend your idle CPU and NET resources to the network for others to use while you earn interest for being a lender.
- **IPFS Storage for Key Documents**: All interactions with key documents in Sqrl, such as the Telos Blockchain Network Operating Agreement, are uploaded and retrieved from the InterPlanetary File System (IPFS).
- **Create Worker Proposals**: Sqrl allows you to create new worker proposal requests on the Telos blockchain. You can also participate in voting on existing worker proposals.
- **Register and Vote on Arbitration**: As the first EOS.IO chain with real on-chain governance support, Sqrl allows anyone to apply to be an arbitrator and voters to elect arbitrators. You can also submit claims and go through the arbitration process using Sqrl.
- **Ratify / Amend Governance Docs**: Sqrl allows you, the voter, to participate in ratifying and amending the Telos governance documents. Let your voice be heard!
- **Works Across Chains**: Sqrl is the first wallet to add support for managing any EOS.IO blockchain in a single interface, such as Telos or EOS.
- **Free User Account Creation**: Sqrl provides a simple wizard that allows new users to create their first Telos account on their own.
- **ScatterJS Core Support**: Version 1.0.0+ of Sqrl now allows users to sign transactions in web-based dApps using ScatterJS, called **Login with Sqrl**. Users of Sqrl no longer needs Scatter Desktop in order to authenticate and interact with their accounts for EOS.IO-based applications.

**CORE FEATURES**:
- **New Key Generation**: You can use Sqrl to generate new EOS.IO public and private key pairs.
- **Block Producer/Proxy Voting**: Select which block producers to support and cast your vote. You can also register/unregister your account as a Proxy.
- **Token Transfers**: Transfer TLOS, EOS or any other token you may have a balance for to another user or exchanges.
- **CPU/Bandwidth Staking**: Stake your TLOS or EOS as either Bandwidth or CPU. This grants rights to resource usage on the network, in addition to conveying weight while voting for block producers.
- **Buy/Sell RAM**: Use your TLOS or EOS tokens to buy or sell RAM at the then market price. RAM allows you to reserve or release storage space on the Telos blockchain.
- **Create Accounts**: Sqrl allows you to create new user accounts in Telos and allocate RAM, Bandwidth or CPU.
- **Simple Contact Management**: You can create a contact database for the Telos accounts you interact with frequently, simplifying the process of sending/receiving tokens on the network.
- **Interact w/ Smart Contracts**: If you would like to interact with smart contracts directly, Sqrl allows you to lookup contracts and call methods defined in the contract's abi.
- **Local Wallet**: Set a password while importing your private key to create a local wallet. Your key will be encrypted locally using this password. This password will be required each time you need to unlock the wallet.
- **Cold Wallet Mode**: If you prefer not to store your keys within the application, simply choose not to set a password. When the application quits, your key will be forgotten.

## Get Sqrl

### Releases

Current 1.1.0 release downloads:

- [Windows Installer](https://github.com/Telos-Foundation/Sqrl/releases/download/1.1.0/win-Sqrl-1.1.0.exe)
- [macOS Package](https://github.com/Telos-Foundation/Sqrl/releases/download/1.1.0/mac-Sqrl-1.1.0.dmg)
- [Linux (AppImage)](https://github.com/Telos-Foundation/Sqrl/releases/download/1.1.0/linux-Sqrl-1.1.0-x86_64.AppImage)

The latest release will always be available on the releases page of this repository:

[https://github.com/Telos-Foundation/Sqrl/releases](https://github.com/Telos-Foundation/Sqrl/releases)

To determine which file you need, if you are a...

- **MacOS User**: Download the DMG (`Sqrl-***.dmg`) file.
- **Windows User**: Download the EXE (`Sqrl-***.exe`) file.
- **Linux User**: Download the Source (`***-.tar.gz`) file.

### Security: Private Keys

When using `Sqrl`, all transactions are signed within the application and your key is never transmitted. If a local wallet password is specified, the application will also save and encrypt your key for future use, using AES-256 encryption. The current password/key encryption scheme can [currently be found here](https://github.com/Telos-Foundation/Sqrl/blob/master/app/shared/actions/wallet.js#L8).

### Endpoints

We offer a public list of nodes within this repository for use with this application:

[https://github.com/Telos-Foundation/Sqrl/blob/master/nodes.md](https://github.com/Telos-Foundation/Sqrl/blob/master/nodes.md)

This list will be updated over time and can be referenced from within the initial connection screen in the app.

### Build it yourself

If you'd rather build the application yourself, please ensure you have nodejs/npm/yarn already installed locally.

**Note**: If you are configuring this Electron application within a Windows development environment, it will involve additional steps.

```
git clone https://github.com/Telos-Foundation/Sqrl.git Sqrl
cd Sqrl
yarn install
```

Then either:

- MacOS: `yarn package`
- Linux: `yarn package-linux`
- Windows: `yarn package-win`
- All: `yarn package-all`

The files built will be located in the `releases` folder within the root project folder.

### Running development mode

```
git clone https://github.com/Telos-Foundation/Sqrl.git Sqrl
cd Sqrl
yarn install
yarn dev
```

### Credits

The development of this application is being led by members of the [Telos Miami](https://eos.miami) team for the [Telos Foundation](https://telosfoundation.io) in an effort to let stakeholders securely manage their EOS.IO-based tokens (TLOS, EOS, etc) and participate in the governance of the Telos blockchain.

`Sqrl` naming credit goes to [Douglas Horn at Goodblock](https://goodblock.io/).

`SqrlJs` + `styling` support provided by [Amplified Telos](https://amplified.software/) development team.

### Release Signatures

To verify the integrity of the releases you download from GitHub, below are the shasum results for each of the binaries:

Signed by [eosmiami on keybase](https://keybase.io/eosmiami)

```
-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA512

shasum -b -a 512 linux-Sqrl-1.1.0-amd64.deb
0f33de7d00f4215ab3968d9450080f4e442c4be3b7890e1d9b5e1d56c4db5b18746d2ca4284554959204a3c87e2c2e60c2bf3899ea1226ee6c74df24c5c6ffca *linux-Sqrl-1.1.0-amd64.deb
shasum -b -a 512 linux-Sqrl-1.1.0-amd64.snap
bd715c5f51fd73264dc6e6dd60f61fd47e29ae107929ab5622e21bd04820ff1ef43d198556c2c067446d1823ed5fe42ff34dcaa340ac6fc5fe2983a54c00bdcd *linux-Sqrl-1.1.0-amd64.snap
shasum -b -a 512 linux-Sqrl-1.1.0-arm64.deb
37cf9333cf7b64525a768f33e1d8e7364c622a1cb3b03f584c99ff6c2ba5311c2f2c41ce80d608fd6881e34da3bb7759c1be0bdb21b09b85c2f453cdc3a9a054 *linux-Sqrl-1.1.0-arm64.deb
shasum -b -a 512 linux-Sqrl-1.1.0-armv7l.deb
05a5eabb98cf3b63f5ae204ee1416bd935a3ad7d3953054384e7263b293ca037a1b23a22fa003da2c28b48c3726fff69f11cec9f986f78270ad67a8eb57bcf6c *linux-Sqrl-1.1.0-armv7l.deb
shasum -b -a 512 linux-Sqrl-1.1.0-i386.deb
03829c80b0935c013025f7ce33e9e03ab3f9b4781390f32f75cac8243504553e834cbacf11760de642ca90ad66a1f909bd1a4b5a0b2be1e95de08033536a2925 *linux-Sqrl-1.1.0-i386.deb
shasum -b -a 512 linux-Sqrl-1.1.0-x86_64.AppImage
5eb0a89918ec538b438ec53fe926b4eda594817578e51ea0155ffc9d0cd71eebf295e377a6b7fb6c4ccbac6d83335aa055d78e575bcfd5f5c6721366483814e7 *linux-Sqrl-1.1.0-x86_64.AppImage
shasum -b -a 512 mac-Sqrl-1.1.0.dmg
9bc105e0a6aa950dfc0fb76d87b238ec34ecbe7ea9e2e8aa203722c46c7462eb449d85cc4e8dbae2a759ad52d798f9e3e0437c284375c759d32f807844c40c0c *mac-Sqrl-1.1.0.dmg
shasum -b -a 512 mac-Sqrl-1.1.0.zip
08ff81e4ba3cad68920cbf43ff1c1eebcf87a05e647922907bdfe0159d680050383744128f3ffab40f2434852c7f6e9516eba6da5385b763b5fc5b50a844b2a6 *mac-Sqrl-1.1.0.zip
shasum -b -a 512 win-Sqrl-1.1.0.exe
e475f7a0134f4191a3034f5653ce05fd1b0229f026fa51c5f6d20ae0a80bb59c0eb2aede542f463d9ddb1f24c327ff427d7d7733ad7e71994ad3f20c58ca0627 *win-Sqrl-1.1.0.exe
-----BEGIN PGP SIGNATURE-----
Version: Keybase OpenPGP v2.1.3
Comment: https://keybase.io/crypto

wsFcBAABCgAGBQJdcqYpAAoJEDT4ke1a0TzT3tIQAKaA5qka8qkaPjiJ8Cg+SZaT
ByZlZbjqcXr13j7E36MaJYOZbuKWV1q+i2hRQ0AJ7UExBAWGX9WNWLZD4UgLreg0
T3256No5UhN8HC5qCRiWfGH7F8YfEOy2IXKDXdJb3h15vU697woTmLCX6rN9zzln
2+j33X5BKX4B0fGZXjMRB1S++srv7+Pzha5h2DWcv/8hzZhKGZUokUMZOHA/ywTO
qTTIwXgaKvZlScQfO+Y9OcTc4QfKBE1blbQS4/z8aYvaj4L75JRy1KaggFu9G4//
BW6z8XKsjgDK/l85PQy/9WoND9gZKGv72WSwl41wXlOor4km8DW8Row1XH2BFLaU
eimT+VKC5AoqQmlky7DYCcJcj4N7rMs3q7AUyddOMuJkhfpuEM+n39QxgrD3RXo9
btMW7jxv+OoTdt39cm+F2znfTjuLfERqQjow//HL0zpKqy95FlqUVBrpa8l5lB1x
oCXM9CgzOOnCweApbKlPPWwum2fxT42ssrsK18Yb5NK9vrJYusTrZENQ82GcP5n3
tGTwsF+2lLmGc+VcwCsTU7zbAPCJ2H2ZZQPJG+JiIVeoEe9BI+kZiMQvcj/+LeqB
udLwt0Joekynd2/iDuI6pnXySnb+VNnE9E8HInYXQ/o/WHqBUlRdqTkPMfd3gwF+
/S+8Q0YPgw+84GmkRcq2
=hHlj
-----END PGP SIGNATURE-----
```