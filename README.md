# hardhat-fund-me-fcc

Learning from FCC and Patrick about Smart Contracts

This contract is for creating a sample funding contract

We have used `Chainlink` to get the price of `ETH` in terms of `USD`. Here funders fund the contract and only the Owner of the contract can withdraw the funds from the contract

---

## Usage

#### Deploy:
`yarn hardhat deploy`

#### Testing:
`yarn hardhat test`

#### Test Coverage:
`yarn hardhat coverage`

---

## Deployment to a Testnet 

#### 1. Setup environment variables:
You'll want to set your `GOERLI_RPC_URL` and `PRIVATE_KEY` as environment variables. You can add them to a .env file
* `PRIVATE_KEY`: The private key of your account (like from metamask).
* `GOERLI_RPC_URL`: This is url of the goerli testnet node you're working with. You can get setup with one for free from [Alchemy](https://www.alchemy.com/)

#### 2. Deploy:
`yarn hardhat deploy --network goerli`

---

## Scripts
After deploy to a testnet or local net, you can run the scripts 

`yarn hardhat run scripts/fund.js`

or

`yarn hardhat run scripts/withdraw.js`




