# StarNotary DAPP
DAPP that allows users to look up, purchase, exchange, and transfer ERC-721 star tokens, known as `Geminorium` (GEM), on the Ethereum blockchain network.

This application is currently deployed to the Rinkeyby test network. The token address used is `3f88a48ee9ec4867b9f6bcca72af2334`.

## Status
The project is still currently under development.

## Getting Started
To get started running a local instance of the DAPP, use the `git clone` command to clone the repository to your local machine:

```
git clone https://github.com/hicks8989/starnotary-dapp
```

This will add the project files to your local machine.

Next, change to the project root folder.

```
cd starnotary-dapp
```

This will bring you to the projects root directory.

The next step is to run the `npm install` command to install all needed project dependencies.

```
npm install
```

Finally, compile the contracts with your truffle console.

```
truffle compile
```

## Requirements
In order to run this project on your local machine, you will need:

* A [MetaMask](https://metamask.io) account installed on your browser.
* [Truffle](https://trufflesuite.com) installed on your machine. You can do this by using the `npm install truffle -g` command.
* [NodeJS](https://nodejs.org) installed on your machine in order to run npm.

## Deployment
In order to deploy your own instance of the project, you will need to:

1. Create a project in [Infura](https://infura.io).
2. Get the project ID for your network of choice.
3. Update the `truffle-config.js` file with your network settings and project ID.

## Testing
In order to run tests for the project, you will need to:

1. Make sure all contracts have been compiled and migrated with the truffle terminal.

```
> truffle develop
truffle(develop)> compile
truffle(develop)> migrate --reset
```

2. Run the truffle test command.

```
truffle(develop)> test
```

## Configuration
In order to get your own instance of the StarNotary DAPP running, certain configuration variables must be set:

* Create a secret file in the root directory insert the mnemonic for your metamask account.

## Project Specifications
Versions of dependencies used to develop, test, and deploy this project:

* openzeppelin-solidity - Version 2.1.2
* Truffle - Version 5.1.27
* Solidity - Version 0.5.16

## Built With
* [NodeJS](https://nodejs.org/) - Backend Language used.
* [Solidity](https://solidity.readthedocs.io/) - Language used to implement smart contracts.