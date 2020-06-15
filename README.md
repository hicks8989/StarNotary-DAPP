# StarNotary
DAPP that allows users to look up, purchase, exchange, and transfer ERC-721 star tokens, known as `Geminorium` (GEM), on the Ethereum blockchain network.

This application is currently deployed to the Rinkeyby test network. Contract address is [`0x82c0f8C20320158d39D396272be576210A3357ce`](https://rinkeby.etherscan.io/tx/0xbec9cd29465e184bca42d466e33a04647d34a9f2563f709e72499567306281f7).

## Getting Started
To get started running a local instance of the DAPP, use the `git clone` command to clone the repository to your local machine:

```
git clone https://github.com/hicks8989/starnotary
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

## Running The Application
In order to run a local instance of the application on your machine, you will need to run the back and front ends seperately.

Instructions for setting up each below:

### Front End
The front end uses `webpack-dev-server` in order to run a local application server on your machine. In order to set this up, the user must:

1. Install `webpack-dev-server` globally on their machine using npm.

```
> npm install webpack-dev-server -g
```

2. Link the `webpack-dev-server` module in the app directory using npm.

```
> cd app
> npm link webpack-dev-server
```

This will setup the `webpack-dev-server` package for the project.

After this, the user needs to install all other dependencies for the front end.

```
> npm install
```

Finally, run the `dev` script in npm to get the local application server running live on the specified port.

```
> npm run dev
```

### Back End
The back end is run using the [Truffle Suite](https://trufflesuite.com) in order to run a local private blockchain. In order to run this instance, the user must:

1. Change to the truffle development console.

```
> truffle develop
```

2. Migrate contracts to be made available for the front end.

```
truffle(develop)> migrate --reset
```

3. Compile contracts.

```
truffle(develop)> compile
```

## Deployment
In order to deploy your own instance of the project, you will need to:

1. Create a project in [Infura](https://infura.io).
2. Get the project ID for your network of choice.
3. Update the `truffle-config.js` file with your network settings and project ID.
4. Make sure you are on a MetaMask account with enough ether for the network of choice and migrate the files.

```
> truffle migrate --reset --network <network>
```

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

* Create a secret file in the root directory and insert the mnemonic for your metamask account.

## Project Specifications
Versions of dependencies used to develop, test, and deploy this project:

* openzeppelin-solidity - Version 2.1.2
* Truffle - Version 5.1.27
* Solidity - Version 0.5.16

## Built With
* [NodeJS](https://nodejs.org/) - Backend Language used.
* [Solidity](https://solidity.readthedocs.io/) - Language used to implement smart contracts.
