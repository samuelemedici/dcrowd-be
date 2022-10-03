# dcrowd_be

Welcome to your new dcrowd_be project and to the internet computer development community. By default, creating a new project adds this README and some template files to your project directory. You can edit these template files to customize your project and to include your own code to speed up the development cycle.

To get started, you might want to explore the project directory structure and the default configuration file. Working with this project in your development environment will not affect any production deployment or identity tokens.

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
