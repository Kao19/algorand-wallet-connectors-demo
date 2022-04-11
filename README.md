# Wallet connector assignment

Complete the wallet connector integration for this sample Dapp. A user should be able to connect to either AlgoSigner, MyAlgo or WalletConnect (with Pera wallet) and perform a payment transaction to another account.

You will need to fill in the wallet integration codes in `wallets.js` and `WalletDemoView.vue`.

## Setup instructions

### 1. Install packages
```
yarn install
```

### 2. Update environement variables
1. Copy `.env.example` to `.env`.
2. Update Algorand Sandbox credentials in `.env` file.

### 3. Setup wallets and test accounts
#### AlgoSigner
1. Download [AlgoSigner browser extension](https://chrome.google.com/webstore/detail/algosigner/kmmolakhbgdlpkjkcjkebenjheonagdm)
2. Create Wallet and accounts on TestNet

#### Add private network to AlgoSigner
1. Follow the instructions [here](https://github.com/PureStake/algosigner/blob/develop/docs/add-network.md) on how to add private network (a.k.a Algorand Sandbox) on AlgoSigner. These are the fields to be added
```
# Display name
Localhost

# Network ID
sandnet-v1

# Network Algod URL
http://localhost:4001

# Network Indexer URL
http://localhost:8980

# Network Headers
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

#### MyAlgo Wallet
1. [Library](https://github.com/randlabs/myalgo-connect) is included in this project.
2. Create TestNet accounts on [MyAlgo](https://wallet.myalgo.com/home)

#### WalletConnect
1. [Library](https://docs.walletconnect.com/quick-start/dapps/node) is included in this the project.

#### Pera Wallet
1. Download [Pera Wallet](https://perawallet.app/)
2. Create TestNet accounts under your Pera Wallet.

#### Fund TestNet accounts
1. Use the [faucet](https://bank.testnet.algorand.network/) to fund your TestNet accounts. You will need to have some funds to maintain account balance and pay transaction fees.

### 4. Use the .env file
```
source .env
```

### 5. Run the Dapp on localhost
```
yarn serve
```