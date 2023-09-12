# How to use ZoKrates with ether.js

Probably due to an update issue, there is a formatting error or constant printing of garbled code when calling Zokrates' verifier contract using ether.js. If you refer to the official documentation for Zokrates, you will see that it doesn't actually work. Thanks to the help of Alberto Viera, we found a solution.

```javascript
const ethers = require('ethers');
const { abi } = require('./compile');
const fs = require('fs');


const providerRPC = {
  development: {
    name: 'moonbeam-development',
    rpc: 'http://localhost:9944',
    chainId: 1281,
  },
  moonbase: {
    name: 'moonbase-alpha',
    rpc: 'https://moonbase-alpha.public.blastapi.io',
    chainId: 1287,
  },
};
const provider = new ethers.providers.JsonRpcProvider(providerRPC.moonbase.rpc, {
  chainId: providerRPC.moonbase.chainId,
  name: providerRPC.moonbase.name,
}); // Change to correct network

const account_from = {
  privateKey: 'YOUR_KEY_DO_NOT_UPLOAD_ONLINE',
};
const contractAddress = 'YOUR_CONTRACT';
const _value = 3;

const proof_source = fs.readFileSync('proof.json', 'utf8');


let wallet = new ethers.Wallet(account_from.privateKey, provider);

const contract = new ethers.Contract(contractAddress, abi, wallet);

const increment = async () => {
  console.log(
    `Calling the increment by ${_value} function in contract at address: ${contractAddress}`
  );


  proof = JSON.parse(proof_source);
  // console.log(proof);
  // console.log(abi);
  const inputStruct = {
    a: {
      X: ethers.BigNumber.from(proof.proof.a[0]),
      Y: ethers.BigNumber.from(proof.proof.a[1]),
    },
    b: {
      X: [ethers.BigNumber.from(proof.proof.b[0][0]), ethers.BigNumber.from(proof.proof.b[0][1])],
      Y: [ethers.BigNumber.from(proof.proof.b[1][0]), ethers.BigNumber.from(proof.proof.b[1][1])],
    },
    c: {
      X: ethers.BigNumber.from(proof.proof.c[0]),
      Y: ethers.BigNumber.from(proof.proof.c[1]),
    }
  }

  const createReceipt =  await contract.verifyTx(inputStruct, [ethers.BigNumber.from(proof.inputs[0])]);

  console.log(createReceipt);
  // await createReceipt.wait();
  // console.log(`Tx successful with hash: ${createReceipt.hash}`);
};

increment();
```

The main issue addressed here is access and type matching.

[1] [Github Repo](https://github.com/only4sim/zk-base-Moonbeam/tree/main)