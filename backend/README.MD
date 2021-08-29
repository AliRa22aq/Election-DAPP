Initial truffle in backend with the following command. <br />
```javascript
truffle init
```

-truffle init this will create a truffle project with truffle-config.js file. Rewrite it.

```javascript
module.exports = {
  networks: {
    development: {
      host: "localhost",
      port: 7545,
      network_id: "*"
    }
},
contracts_directory: './contracts/',
contracts_build_directory: '../frontend/src/abis/',
compilers: {
  solc: {
    version: "^0.8.0",
    optimizer: {
      enabled: true,
      runs: 200
    }
  }
}
}```


Now we need to deploy this smart contract to Ganache

-touch migrations/2_deploy_contracts.js

This file tells Truffle to to deploy our smart contract to the blockchain. Also, note that the migration files are numbered so that Truffle knows which order to run them in.

add the following const Marketplace = artifacts.require("Marketplace");

truffle migrate --reset smart contract tests $ mkdir test $ touch test/Marketplace.test.js passed, add function- create product and variables to contract test again add tools to our test suite

require('chai') .use(require('chai-as-promised')) .should()

write tests and test npm i "chai": "^4.3.4", "chai-as-promised": "^7.1.1",

add function- sell product and variables to contract add test truffle migrate --reset done

frontend mkdir frontend npx create-react-app npm i web3 Connect Metamask to our Ganache personal blockchain instance import Web3 from 'web3' instantiates web3.
