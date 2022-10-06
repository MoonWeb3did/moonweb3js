# Moon Web3 Identity SDK

Nodejs SDK

Npm: https://www.npmjs.com/package/domainchainjs

Before installing the package you need to check and be sure to install the packages below:

```
npm install web3 
```

Install Package

```
npm install domainchainjs
```

Call 
```
const domainchainjs = require('domainchainjs');
```

Install:

Chain Supported: moonbeam, moonriver

```
const moonbeam = 
{
	"rpcUrl": "https://rpc.api.moonbeam.network/",
	"contractAddress": "0x819B997a2f711eC1Ee998cB2DF5a6B2c4be1B575"		
}

const moonriver = 
{
	"rpcUrl": "https://rpc.api.moonriver.moonbeam.network",
	"contractAddress": "0xa1019535e6b364523949eaf45f4b17521c1cb074"
}

// your domains
const _domain = "moonbeam.moon"; // moonbeam.glmr
//const _domain = "moonriver.movr";
	
// resolve domain to get the address of the owner.
const owner = await sdk.getOwner(_domain);

console.log(owner);

// your address
const _address = "xxx";

// get a domain default from a user's address, requiring the user to set the default domain name initially.
const domain = await sdk.getDomain(_address);

console.log(domain);
```
Pls update test.js for specific instructions

Thanks!



