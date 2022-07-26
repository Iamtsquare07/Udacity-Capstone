# Capstone: Real Estate Marketplace
* v1.0.1
* By Tsquare07

### Dependencies
For this project, you will need to have:
1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)
```bash
# Check Node version
node -v
# Check NPM version
npm -v
```


2. **Truffle v5.X.X** - A development framework for Ethereum. 
```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Verify the version
truffle version
```


### Run the application
1. NPM install
```bash
# Remove the node_modules  
# remove packages
rm -rf node_modules
# clean cache
npm cache clean
rm package-lock.json
# install all modules listed as dependencies in package.json
npm install
```

2. Start Truffle by running
```bash
# For starting the development console
cd eth-contracts
truffle develop
# truffle console

# For compiling the contract, inside the development console, run:
compile

# For migrating the contract to the locally running Ethereum network, inside the development console
migrate --reset

# For running unit tests the contract, inside the development console, run:
test
```
# Deployment on rinkeby

Run `truffle migrate --network rinkeby --reset --compile-all`

* Deployed contracts on Rinkeby

The following contracts provide the Zero-Knowledge proof process:

* Verifier: `eth-contracts/contracts/SquareVerifier.sol`

            `0xfAc43c172958326340C240A184c99050Dfd5d6C1`

             https://rinkeby.etherscan.io/address/0xfAc43c172958326340C240A184c99050Dfd5d6C1

* SolnSquareVerifier: `eth-contracts/contracts/SolnSquareVerifier.sol`

            `0xEbC6b846064f7af155AA3551b5699016A8aDBFb7`

            https://rinkeby.etherscan.io/address/0xEbC6b846064f7af155AA3551b5699016A8aDBFb7

The SquareVerifier.sol contract is created using Zokrates, see below for details.

# Contracts ABI

Contracts' ABIs can be found in the following files:
```
eth-contracts/build/contracts/ERC721Mintable.json
eth-contracts/build/contracts/SquareVerifier.json
eth-contracts/build/contracts/SolnSquareVerifier.json
```
* OpenSea marketplace
https://testnets.opensea.io/collection/real-estate-200899
