
## Start a new DApp with Truffle’s React Box

mkdir openlaw-api-tutorial
cd openlaw-api-tutorial
truffle unbox react

Test the Truffle’s React Box in Ganache

run ganache

update files 
- truffle-cofig.js (add network config  host: "127.0.0.1", port: 7545,)
- client/src/utils/getWeb3.js (line 29)

Migrate account in Metamask with Ganche mnemonic



Contract compilation and deploy

truffle compile
truffle migrate --reset

Run Dapp

on /client folder
npm run start

-------------
## OpenLaw API Sale Agreement

OpenLaw template name: “Sale Agreement - LV”


Once the Truffle’s React Box works follow this tutorial:

OpenLaw  — Build a complete Dapp with the OpenLaw API + Truffle + React.js.
https://medium.com/@OpenLawOfficial/openlaw-api-tutorial-build-a-complete-dapp-with-the-openlaw-api-truffle-react-js-d064717ad41d?fbclid=IwAR1GTEXx2p9oezQAgyN9sHWvA2dLOioPewi0Y-NAnnjIBf9U6CjiHZ9f2D8

In the .env file create a MNEMONIC and INFURA_API_KEY variable. It should be your own mnemoic and Infura API Key (Note: do not put quotes around the mnemonic).

- If there is an error when compiling the contract with truffle-hdwallet-provider, try to execute this:
  npm install truffle-hdwallet-provider
instead of this:
  npm install truffle-hdwallet-provider@web3-one 

- Contract compilation and deploy

rm -r build/
truffle compile
truffle migrate --reset --network rinkeby

- Run Dapp

on /client folder
npm run start

Test Data

Seller Ethereum Address
0xE91B4c3F95DFe54c18874771C7d1C9EE3AE00b8f
theotherguytotest@gmail.com

Buyer Ethereum Address
0xFE3e5D87904EC3A15020232C88b653a997Ffaad0
luisvid@gmail.com
