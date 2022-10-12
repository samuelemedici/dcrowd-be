# dCROWD - bridging people around events

### Welcome to dCrowd and the Internet Computer development community!
![dCrowd_logo](https://user-images.githubusercontent.com/98580234/194874704-5bcefb6a-dad8-4b79-ac5c-55e96592a90c.jpeg)


# ABOUT dCROWD
_**dCrowd**_ is a decrentralized crowdfunding platform that allows event planners all over the world to fund their events through NFT sales. In the case of a successful crowdfunding, the non-fungible tokens offered as perks will be used as tickets to grant access to the event itself, be it a webinar, a real-life or even a Metaverse occurrence. The highlight of _**dCrowd**_ is to be based on [Dfinity](https://dfinity.org) and make smart use of its cross-chain technology. As of October 2022, dCrowd supports a Dfinity Internet Computer ICP-ETH Etherum bridge, and it aims at extending the payout opportunity as more blockchain assets become IC-compatible with Dfinity's establishment of new bridges.

# UI - let's keep it simple
The dApp is as straightforward and essential as it can be. It consists of:
- **Dashboard:** to browse all the to-be-funded events and discover what is trending in the world(s)
- **Event detail:** to find out more about the event you are considering funding
- **Event creation section:** where the organizer can fill in details about their event and submit it to dCrowd
- **Wallet connection:** where users connect their PlugWallets

### dCrowd - Dashboard
![dCrowd_UI_dashboard](https://user-images.githubusercontent.com/98580234/194858783-987b6cf8-7437-4b69-b5be-4f7ada3333db.jpeg)

### dCRowd - Event detail
![dCrowd_UI_event_detail](https://user-images.githubusercontent.com/98580234/194860902-a26911b1-3c64-40be-acec-16e7567af822.jpeg)

### dCrowd - PlugWallet connection
<img width="492" alt="Screenshot 2022-10-10 at 16 32 27" src="https://user-images.githubusercontent.com/98580234/194891083-c3fded4c-0ea1-466e-9470-79bb6caac18f.png">

### dCrowd - Success message
<img width="930" alt="Screenshot 2022-10-10 at 16 33 31" src="https://user-images.githubusercontent.com/98580234/194891226-279a7784-7d26-4d69-8f01-39fb0d44f1a9.png">


# HOW dCROWD WORKS
_**dCrowd**_ is a full responsive web platform which users can interface with by authenticating through Internet Identity and connecting a wallet using the tools provided by PlugWallet, a wallet plugin that allows storing and managing NFTs and tokens on the Internet Computer.

The development stack includes NextJS, a NodeJS based-technology which utilizes cutting-edge features such as Server-Side Rendering, Typescript and Tailwind framework. In order to operate, the web application communicates with a backend [canister](https://github.com/dfinity/sdk) developed in Motoko and deployed directly on the Internet Computer network. The canister is based on the DIP721 NFT standard, which is the IC-adapted counterpart of the ERC721 NFT Standard for Ethereum. 

Being the whole crosschain experience made possible by the integration of Terabethia, a cross chain protocol that allows asset mirroring between the Internet Computer and Ethereum blockchains, _**dCrowd**_ allows easy connection to two key technologies to interact with these ecosystems: [PlugWallet](https://plugwallet.ooo) - Internet Computer crypto wallet - and [WalletConnect](https://walletconnect.com) to facilitate the use of any non-ICP-specific wallet within the platform.

By default an event planner's NFT are minted on the IC but, thanks to the ICP-ETH bridge, it is possible to purchase them in either ICP or ETH. Users will receive live conversion data between ETH and ICP through the connection with an external API (e.g. CoinGeko).
Etherum users will be granted the opportunity of buying IC-standard NFTs by easily exchanging ETH with ICP, through a ETH burn/retrieve process. In this case, users will be redirected to Terabethia which will process the currency swap. Once successful, dCrowd will make a balance check on the user’s PlugWallet and process the transaction.

### WalletConnect & PlugWallet connections
![DIAGRAM_WalletConnection](https://user-images.githubusercontent.com/98580234/194863856-a1d2506c-0e34-4b63-8269-ee65a34d9131.png) ![PlugWallet_connection](https://user-images.githubusercontent.com/98580234/194862499-a353d21b-0ffa-4655-afde-ae14f34a6f57.png)


### NFT minting & transaction
![NFT_minting](https://user-images.githubusercontent.com/98580234/194867490-d89d208b-911b-42cd-ac85-bb27595914b6.png)
![buyNFT_swap](https://user-images.githubusercontent.com/98580234/194864147-cb6b2af1-d7b1-4f23-a5dc-e4777f888c69.png)


### NFT QR code generation (where needed)
In order to use the NFTs as tickets, some event may require a QR code to be read to grant access.
![eventQRcode](https://user-images.githubusercontent.com/98580234/194864440-44d86cd0-ed00-4a9c-ac15-c9a42d2d099c.png)

# ATTACK PREVENTION
To ensure the platform’s safety, continuous auditing is planned on each smart contract from the pre-deployment phase on, including the prompt notice of abnormal transactions and assuring an insurance fund in the budget plan. Planning ahead on further platform enhancements, it will be possible to implement a Motoko compatible version of the static analysis framework based on the current Solidity’s Slither.

<img width="639" alt="Screenshot 2022-10-12 at 20 10 39" src="https://user-images.githubusercontent.com/98580234/195417353-4dddccb5-e639-47d7-aaae-c16974690417.png">

# BEHIND THE IDEA, BEYOND TECH
_**dCrowd**_'s structure and functioning are based on fine market research. A survey was conducted from a pool of participant selected via random sampling procedure. Among the 70 participants, 68 filled the survey with complete and analysable results. The age of the majority of respondents was between 26 and 30 years old (36.8%), followed by the lowest age range (21-25, 33.8%) and, finally, by the category of age of 50 y/o or more (20.6%).

[**CLICK HERE TO ACCESS THE FULL REPORT**](https://github.com/samuelemedici/dcrowd-be/files/9745900/d-Crowd.survey.potential.use.pdf)
<img width="859" alt="Screenshot 2022-10-10 at 14 20 18" src="https://user-images.githubusercontent.com/98580234/194866471-faa2a119-9f94-4630-a797-e88815ff4dda.png"> <img width="862" alt="Screenshot 2022-10-10 at 14 20 56" src="https://user-images.githubusercontent.com/98580234/194866234-d41869f1-2128-40ac-a739-f5bbae079a2c.png">


# DIRECTORY STRUCTURE

To learn more before you start working with dcrowd_be, see the following documentation available online:

- [Quick Start](https://sdk.dfinity.org/docs/quickstart/quickstart-intro.html)
- [SDK Developer Tools](https://sdk.dfinity.org/docs/developers-guide/sdk-guide.html)
- [Motoko Programming Language Guide](https://sdk.dfinity.org/docs/language-guide/motoko.html)
- [Motoko Language Quick Reference](https://sdk.dfinity.org/docs/language-guide/language-manual.html)
- [JavaScript API Reference](https://erxue-5aaaa-aaaab-qaagq-cai.raw.ic0.app)

If you want to start working on your project right away, you might want to try the following commands:

```bash
cd dcrowd_be/
dfx help
dfx canister --help
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --clean --background

# Deploys your canisters to the replica
dfx deploy
```

#### Ledger / Wallet

Get ledger balance

```bash
dfx ledger --network ic balance`
```

Check cycles balance

```bash
dfx wallet --network ic balance`
```

Get wallet id

```bash
dfx identity --network ic get-wallet`
```

Set wallet

```bash
dfx identity --network=ic set-wallet <canister id>
```

#### Identity

Get current identity Principal

```bash
dfx identiy get-principal
```

In order to call minting canister try

```bash
dfx canister call nftController name
```

#### Utilities

Transfer NFT from one Principal to another

```bash
dfx canister call nftController transferFrom '(principal "first_principal", principal "second_principal", tokenId)
```
