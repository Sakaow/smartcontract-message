# smartcontract-message
# Smart Contract Inbox Project README

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Testing](#testing)


## Introduction
This is a Smart Contract Inbox project built using Ethereum smart contracts and web3.js. The project allows you to send and receive messages via a simple Ethereum smart contract. It also incorporates Ganache for local testing and Infura Ethereum Sepolia Faucet as a testnet for remote testing.

## Prerequisites
Before you begin, ensure you have met the following requirements:
- Node.js and npm installed
- Ganache installed
- Metamask extension installed in your browser
- An Infura account for Ethereum testnet access
- An Ethereum wallet (e.g., MetaMask) for transaction signing

## Installation
To install and set up this project, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/Sakaow/smartcontract-message.git
   ```

2. Change to the project directory:

   ```bash
   cd inbox
   ```

3. Install project dependencies:

   ```bash
   npm install
   ```

## Configuration
To configure the project, follow these steps:

1. Create a `.env` file in the project root directory to store your secret values. You can use the provided `.env.example` as a template.

   ```bash
   cp .env.example .env
   ```

2. Open the `.env` file and fill in the following values:
   - `MNEMONIC`: Your 12-word mnemonic phrase for your Ethereum wallet.
   - `INFURA_API_KEY`: Your Infura API key for connecting to the Ethereum network.   

## Usage
To use the Smart Contract Inbox, you can perform the following actions:

1. Compile and deploy the smart contract to the local Ganache network:

   ```bash
   npm run deploy-local
   ```

2. Deploy the smart contract to the Ropsten testnet (using Infura):

   ```bash
   npm run deploy-ropsten
   ```

3. Interact with the deployed contract by sending and receiving messages:

   ```bash
   npm run send-message "Your message here"
   npm run get-message
   ```

4. Explore the `inbox.js` script to see how to interact with the smart contract.

## Testing
This project uses Mocha for testing. To run the tests, execute the following command:

```bash
npm test
```

Make sure you have Ganache running locally or are connected to the Ethereum testnet via Infura when running the tests.
