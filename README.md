# How to Create an NFT Bound Account (ERC-6551)


## Clone Example Monorepo

To begin, clone the `qn-guide-examples` repo, navigate to this project's directory and open the project directory in a code editor (VS code in this case).

```bash
git clone git@github.com:FadhilMulinya/ERC6551.git
cd ERC6551/ethereum/erc-6551
code .
```

Install project dependencies by running:

```sh
npm install
```

Create an **.env** file and fill in the environment variable with your private key and RPC endpoint:

```sh
RPC_URL=
PRIVATE_KEY=
```

To deploy contracts, we'll need to execute the **createAccount.js** script located in `scripts`:

```
npx hardhat run --network sepolia scripts/createAccount.js
```

To interact with your Token Bound Account, open the **interactAccount.js** file within `scripts` and replace the `nftContractAddress` and `tokenBoundAccountAddress` variables with proper values. These values were printed out in the previous script. 

Then, save the file and execute the script:

```sh
npx hardhat run --network sepolia scripts/interactAccount.js
```

Each script will output logs regarding the events that have occurred.
