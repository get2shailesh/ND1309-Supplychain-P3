# ND1309-Supplychain-P3

Udacity Block chain Developer course – project 3

Ethereum DAPP for COFFEE SUPPLY CHAIN 

This project is about creating a DApp supply chain solution backed by the Ethereum platform and to architect smart contracts that manage specific user permission controls as well as contracts that track and verify a product’s authenticity. It has front end in HTML/Java script and it uses tools like Solidity, Infura, Ganache, Mocha, Chai, Truffle etc. to develop backend based on Ethereum blockchain. 

UML – Activity diagram for Coffee harvesting process used in this project:

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/UML-DrawIO/activitydiagram.png

UML – Sequence diagram for coffee supply chain project.

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/UML-DrawIO/sequencediagram.png

State diagram for coffee supply chain project

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/UML-DrawIO/statediagram.png

Domain model Interfaces

AccessControl - Collection of Contracts: These contracts manages the various addresses and constraints for operations that can be executed only by specific roles.

Base - SupplyChain.sol: This is where we define the most fundamental code shared throughout the core functionality. This includes our main data storage, constants and data types, plus internal functions for managing these items.

Core - Ownable.sol: is the contract that controls ownership and transfer of ownership.

UML – Class diagram for the coffee supply chain project

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/UML-DrawIO/classdiagram.png

The environment set up for the project and versions are as follows:
--------------------------------------------
Truffle version and other libraries used
--------------------------------------------
blunionsolutions@Blunion MINGW64 ~/Documents/02-CRYPTO-DEFI/Blockchain Developer/project-code/project3code/SupplyChainP3
$ truffle version
Truffle v5.7.3 (core: 5.7.3)
Ganache v7.7.3
Solidity v0.5.16 (solc-js)
Node v18.12.1
Web3.js v1.8.1

$ ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
Ganache CLI v6.12.2 (ganache-core: 2.13.2)

Available Accounts
==================
(0) 0x27D8D15CbC94527cAdf5eC14B69519aE23288B95 (100 ETH)
(1) 0x018C2daBef4904ECbd7118350A0c54DbeaE3549A (100 ETH)
(2) 0xCe5144391B4aB80668965F2Cc4f2CC102380Ef0A (100 ETH)
(3) 0x460c31107DD048e34971E57DA2F99f659Add4f02 (100 ETH)
(4) 0xD37b7B8C62BE2fdDe8dAa9816483AeBDBd356088 (100 ETH)
(5) 0x27f184bdc0E7A931b507ddD689D76Dba10514BCb (100 ETH)
(6) 0xFe0df793060c49Edca5AC9C104dD8e3375349978 (100 ETH)
(7) 0xBd58a85C96cc6727859d853086fE8560BC137632 (100 ETH)
(8) 0xe07b5Ee5f738B2F87f88B99Aac9c64ff1e0c7917 (100 ETH)
(9) 0xBd3Ff2E3adEd055244d66544c9c059Fa0851Da44 (100 ETH)

Private Keys
==================
(0) 0x9137dc4de37d28802ff9e5ee3fe982f1ca2e5faa52f54a00a6023f546b23e779
(1) 0x18911376efeff48444d1323178bc9f5319686b754845e53eb1b777e08949ee9b
(2) 0xf948c5bb8b54d25b2060b5b19967f50f07dc388d6a5dada56e5904561e19f08b
(3) 0xfad19151620a352ab90e5f9c9f4282e89e1fe32e070f2c618e7bc9f6d0d236fb
(4) 0x19d1242b0a3f09e1787d7868a4ec7613ac4e85746e95e447797ce36962c7f68b
(5) 0x3bb675f8c07099816e23a3e283090cfb0f793ab625b73ca51a2d027a3c1f2d0e
(6) 0x0faf45306c7daf14d86c266690ce54490e8c0104154cafa87d9e93724efc239d
(7) 0xf2a921dee0ebd7bfaba1a271bcd48c99baa6341a1cdf84ba843521a5555e0273
(8) 0x62734594840dade92a24448c8f676cc3c59fd68909837303417295f2c0f27963
(9) 0xc29afb730456eb83415046550faf8065c8531765396156db8d97fd1fd64c6a6e

HD Wallet
==================
Mnemonic:      spirit supply whale amount human item harsh scare congress discover talent hamster
Base HD Path:  m/44'/60'/0'/0/{account_index}

Gas Price
==================
20000000000

Gas Limit
==================
6721975

Call Gas Limit
==================
9007199254740991

Listening on 127.0.0.1:8545

IPFS was not used for this project.

-----------------------------------------------------
Log of goerli deployment:
-----------------------------------------------------
blunionsolutions@Blunion MINGW64 ~/Documents/02-CRYPTO-DEFI/Blockchain Developer/project-code/project3code/SupplyChainP3
$ truffle migrate --reset --network goerli

Compiling your contracts...
===========================
> Compiling .\contracts\Migrations.sol
> Compiling .\contracts\coffeeaccesscontrol\ConsumerRole.sol
> Compiling .\contracts\coffeeaccesscontrol\DistributorRole.sol
> Compiling .\contracts\coffeeaccesscontrol\FarmerRole.sol
> Compiling .\contracts\coffeeaccesscontrol\RetailerRole.sol
> Compiling .\contracts\coffeeaccesscontrol\Roles.sol
> Compiling .\contracts\coffeebase\SupplyChain.sol
> Compiling .\contracts\coffeecore\Ownable.sol
> Artifacts written to C:\Users\blunionsolutions\Documents\02-CRYPTO-DEFI\Blockchain Developer\project-code\project3code\SupplyChainP3\build\contracts
> Compiled successfully using:
   - solc: 0.5.16+commit.9c3226ce.Emscripten.clang


Starting migrations...
======================
> Network name:    'goerli'
> Network id:      5
> Block gas limit: 30000000 (0x1c9c380)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0xbc65548259358b0f5d0e2c8168803f27386852bf4b13726761832037acdf45a0
   > Blocks: 0            Seconds: 0
   > contract address:    0x91231544AfEdEb1E098f92Ef82Cac5bBEc0fa4D1
   > block number:        8462387
   > block timestamp:     1675951176
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.198105360363313081
   > gas used:            226537 (0x374e9)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.001894639636686919 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8462388)
   > confirmation number: 2 (block: 8462389)
   > confirmation number: 3 (block: 8462390)
   > confirmation number: 4 (block: 8462391)
   > confirmation number: 5 (block: 8462392)
   > confirmation number: 6 (block: 8462393)
   > confirmation number: 7 (block: 8462394)
   > confirmation number: 8 (block: 8462395)
   > confirmation number: 9 (block: 8462396)
   > confirmation number: 10 (block: 8462397)
   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.001894639636686919 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x092c85536bb6d97f008095dc097827bcbfff3522e75354177f24db19c4c9225a
   > Blocks: 0            Seconds: 20
   > contract address:    0x4ed91962D9F898727F1dF3dF82E0a0B7277AEd5f
   > block number:        8462399
   > block timestamp:     1675951332
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.195157673866045992
   > gas used:            306684 (0x4adfc)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002564948164483908 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8462400)
   > confirmation number: 2 (block: 8462401)
   > confirmation number: 3 (block: 8462402)
   > confirmation number: 4 (block: 8462403)
   > confirmation number: 5 (block: 8462404)
   > confirmation number: 6 (block: 8462405)
   > confirmation number: 7 (block: 8462406)
   > confirmation number: 8 (block: 8462407)
   > confirmation number: 9 (block: 8462408)
   > confirmation number: 10 (block: 8462409)

   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x9f44410860ac7a2bf9ced5c34d3f77032946a0017995609e35c47d0ba521dfd2
   > Blocks: 1            Seconds: 20
   > contract address:    0xFb5a9d39E8fB475f4A970A92C6594BA397f74988
   > block number:        8462411
   > block timestamp:     1675951524
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.19254771340544865
   > gas used:            312066 (0x4c302)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002609960460597342 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8462412)
   > confirmation number: 2 (block: 8462413)
   > confirmation number: 3 (block: 8462414)
   > confirmation number: 4 (block: 8462415)
   > confirmation number: 5 (block: 8462416)
   > confirmation number: 6 (block: 8462417)
   > confirmation number: 7 (block: 8462418)
   > confirmation number: 8 (block: 8462419)
   > confirmation number: 9 (block: 8462420)
   > confirmation number: 10 (block: 8462421)

   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0xb35d0b8cf14c7ac08c49bd658923bacfd9c84cf7294087018235e70514f15c98
   > Blocks: 0            Seconds: 8
   > contract address:    0x9D5A39f3c899B8072Be569ba86E47fd8E06b3cBf
   > block number:        8462422
   > block timestamp:     1675951704
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.189937652582987064
   > gas used:            312078 (0x4c30e)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002610060822461586 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8462423)
   > confirmation number: 2 (block: 8462424)
   > confirmation number: 3 (block: 8462425)
   > confirmation number: 4 (block: 8462426)
   > confirmation number: 5 (block: 8462427)
   > confirmation number: 6 (block: 8462428)
   > confirmation number: 7 (block: 8462429)
   > confirmation number: 8 (block: 8462430)
   > confirmation number: 9 (block: 8462431)
   > confirmation number: 10 (block: 8462432)

   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x1b1946ef507a201f35cb80a9c7b681601cde87f3bcf1d8babef077bd4f2a2598
   > Blocks: 2            Seconds: 17
   > contract address:    0x37a6afEC0589dBcAbb5e084652361156401Cc7CE
   > block number:        8462434
   > block timestamp:     1675951860
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.187327591760525478
   > gas used:            312078 (0x4c30e)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002610060822461586 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8462435)
   > confirmation number: 2 (block: 8462436)
   > confirmation number: 3 (block: 8462437)
   > confirmation number: 4 (block: 8462438)
   > confirmation number: 5 (block: 8462439)
   > confirmation number: 6 (block: 8462440)
   > confirmation number: 7 (block: 8462441)
   > confirmation number: 8 (block: 8462442)
   > confirmation number: 9 (block: 8462443)
   > confirmation number: 10 (block: 8462444)

   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0x920698ce993a5121cdb6afe7bd7fc92d0602e831d3b3a7b9ff3a139bd9b0aebf
   > Blocks: 0            Seconds: 4
   > contract address:    0x8c7E1c25df2e4f51d8A8F5b4c1888401C33A2F60
   > block number:        8462445
   > block timestamp:     1675952028
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.161526329522994722
   > gas used:            3084988 (0x2f12bc)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.025801262237530756 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8462446)
   > confirmation number: 2 (block: 8462447)
   > confirmation number: 3 (block: 8462448)
   > confirmation number: 4 (block: 8462449)
   > confirmation number: 5 (block: 8462450)
   > confirmation number: 6 (block: 8462451)
   > confirmation number: 7 (block: 8462452)
   > confirmation number: 8 (block: 8462453)
   > confirmation number: 9 (block: 8462454)
   > confirmation number: 10 (block: 8462455)
   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.036196292507535178 ETH

Summary
=======
> Total deployments:   6
> Final cost:          0.038090932144222097 ETH

------------------------------------------
Log of test:
------------------------------------------

blunionsolutions@Blunion MINGW64 ~/Documents/02-CRYPTO-DEFI/Blockchain Developer/project-code/project3code/SupplyChainP3
$ truffle test
Using network 'development'.


Compiling your contracts...
===========================
> Compiling .\contracts\Migrations.sol
> Compiling .\contracts\coffeeaccesscontrol\ConsumerRole.sol
> Compiling .\contracts\coffeeaccesscontrol\DistributorRole.sol
> Compiling .\contracts\coffeeaccesscontrol\FarmerRole.sol
> Compiling .\contracts\coffeeaccesscontrol\RetailerRole.sol
> Compiling .\contracts\coffeeaccesscontrol\Roles.sol
> Compiling .\contracts\coffeebase\SupplyChain.sol
> Compiling .\contracts\coffeecore\Ownable.sol
> Artifacts written to C:\Users\BLUNIO~1\AppData\Local\Temp\test--21712-7CC6S5AALYmX
> Compiled successfully using:
   - solc: 0.5.16+commit.9c3226ce.Emscripten.clang
ganache-cli accounts used here...
Contract Owner: accounts[0]  0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
Farmer: accounts[1]  0x018C2daBef4904ECbd7118350A0c54DbeaE3549A
Distributor: accounts[2]  0xCe5144391B4aB80668965F2Cc4f2CC102380Ef0A
Retailer: accounts[3]  0x460c31107DD048e34971E57DA2F99f659Add4f02
Consumer: accounts[4]  0xD37b7B8C62BE2fdDe8dAa9816483AeBDBd356088


  Contract: SupplyChain
    ✔ Testing smart contract function harvestItem() that allows a farmer to harvest coffee (562ms)
    ✔ Testing smart contract function processItem() that allows a farmer to process coffee (294ms)
    ✔ Testing smart contract function packItem() that allows a farmer to pack coffee (270ms)
    ✔ Testing smart contract function sellItem() that allows a farmer to sell coffee (297ms)
    ✔ Testing smart contract function buyItem() that allows a distributor to buy coffee (320ms)
    ✔ Testing smart contract function shipItem() that allows a distributor to ship coffee (255ms)
    ✔ Testing smart contract function receiveItem() that allows a retailer to mark coffee received (360ms)
    ✔ Testing smart contract function purchaseItem() that allows a consumer to purchase coffee (291ms)
    ✔ Testing smart contract function fetchItemBufferOne() that allows anyone to fetch item details from blockchain (78ms)
    ✔ Testing smart contract function fetchItemBufferTwo() that allows anyone to fetch item details from blockchain (86ms)


  10 passing (3s)


Results:

Task 1: Boiler plate code has been successfully modified per the project instructions and the code for the project is uploaded here:

Task 2: All test cases were successful. Log provided above.

Task 3: Contract was deployed on Goerli network. Following is the latest:

•	“Contract Address” on the Goerli Network:

•	https://goerli.etherscan.io/address/0x8c7E1c25df2e4f51d8A8F5b4c1888401C33A2F60

•	Contract: 0x8c7E1c25df2e4f51d8A8F5b4c1888401C33A2F60

[The following details are from the initial contract deployment for initial submission, as per the feedback, I have re-deployed the contract]

•	Initial “Contract Address” on the Goerli Network:

https://goerli.etherscan.io/address/0xFB1e9CF1D94fb443a07aA84DB5FAd869784dCa55

•	Initial Contract for reference: 0xFB1e9CF1D94fb443a07aA84DB5FAd869784dCa55]

Task 4: The application was successfully invoked to perform certain functions.

Account set up in Metamask using mnemonic provided (I had collected GoerliETH for this project using testnet faucets and distributed across the accounts for using it.) 

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/images/AccountSetup.png

Task 5: The application was successfully invoked and started.

Running command npm run dev invokes the coffee app and it is connected to owner account for ETH transactions.

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/images/UIview.png

Task 6: Transactions tested.



