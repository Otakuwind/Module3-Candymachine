# Metacrafters Candy Machine Challenge
## Overview
In this challenge, we created a Candy Machine, a system designed to manage and dispense NFTs (Non-Fungible Tokens) on the Solana blockchain. This README will guide you through the setup, usage, and development process.

## Prerequisites

Before you begin, ensure you have the following software installed:

* Node.js (version 14.x or higher)
* npm or yarn
* Solana CLI

## Installation

To get started, clone the repository and install the necessary dependencies:

`git clone` "https://github.com/metacrafters/candy-machine-challenge.git
cd candy-machine-challenge"

`npm install`
 or
`yarn install`

## Usage
### Setting Up the Environment

* Create a Solana Wallet: Generate a new wallet or use an existing one. Save the keypair file securely.
`solana-keygen new --outfile ~/my-solana-wallet.json`

* Airdrop SOL: Fund your wallet with SOL for transactions (on the devnet).
`solana airdrop 2 ~/my-solana-wallet.json`

* Deploying the Candy Machine
* Configure Environment Variables: Create a `.env` file in the project root and add the necessary configuration.

WALLET_KEYPAIR_PATH=~/my-solana-wallet.json
NETWORK=devnet

* Upload Assets: Prepare your NFT assets (images, metadata) and upload them using the provided script.

`npm run upload-assets`
or
`yarn upload-assets`

* Create Candy Machine: Initialize and deploy the Candy Machine using the following command:

    `npm run create-candy-machine`
    or
    `yarn create-candy-machine`

* Minting NFTs

Users can mint NFTs from your Candy Machine by running the mint command:


`npm run mint-nft`
or
`yarn mint-nft`

## Configuration

The config.json file contains the configuration for your Candy Machine. You can customize the following settings:

    Price: The cost of minting an NFT.
    Number of NFTs: The total supply of NFTs available.
    Symbol: The symbol for your NFTs.
    Creators: The list of creators and their shares.

## Contributing

To make contributions! Please fork the repository and create a pull request with your changes.
