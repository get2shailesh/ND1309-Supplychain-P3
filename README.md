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
   > transaction hash:    0x83f4231fec4fce62167a340cb4b78dcb326056d65dfa8bc869e154741172ceed
   > Blocks: 0            Seconds: 4
   > contract address:    0x3A1Dd7228022B06dFBEB7586b4d58f667e37E96D
   > block number:        8463729
   > block timestamp:     1675970904
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.148105360363313081
   > gas used:            226537 (0x374e9)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.001894639636686919 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463730)
   > confirmation number: 2 (block: 8463731)
   > confirmation number: 3 (block: 8463732)
   > confirmation number: 4 (block: 8463733)
   > confirmation number: 5 (block: 8463734)
   > confirmation number: 6 (block: 8463735)
   > confirmation number: 7 (block: 8463736)
   > confirmation number: 8 (block: 8463737)
   > confirmation number: 9 (block: 8463738)
   > confirmation number: 10 (block: 8463739)
   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.001894639636686919 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x8020a769753981bd62d6a908249e27d3e1425aec4129bde825ddcca55acb946a
   > Blocks: 0            Seconds: 32
   > contract address:    0xD15070122C755989BB8d701d1Da1753637Ff30F6
   > block number:        8463741
   > block timestamp:     1675971132
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.145157673866045992
   > gas used:            306684 (0x4adfc)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002564948164483908 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463742)
   > confirmation number: 2 (block: 8463743)
   > confirmation number: 3 (block: 8463744)
   > confirmation number: 4 (block: 8463745)
   > confirmation number: 5 (block: 8463746)
   > confirmation number: 6 (block: 8463747)
   > confirmation number: 7 (block: 8463748)
   > confirmation number: 8 (block: 8463749)
   > confirmation number: 9 (block: 8463750)
   > confirmation number: 10 (block: 8463751)

   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x67d9e723109bd395148ab45becbeadf02800b4bd19f9f04dac4c2b92c3408ade
   > Blocks: 0            Seconds: 8
   > contract address:    0xEff45f969Aaf48E3703E587f7D9E7c41e6845822
   > block number:        8463752
   > block timestamp:     1675971276
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.14254771340544865
   > gas used:            312066 (0x4c302)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002609960460597342 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463753)
   > confirmation number: 2 (block: 8463754)
   > confirmation number: 3 (block: 8463755)
   > confirmation number: 4 (block: 8463756)
   > confirmation number: 5 (block: 8463757)
   > confirmation number: 6 (block: 8463758)
   > confirmation number: 7 (block: 8463759)
   > confirmation number: 8 (block: 8463760)
   > confirmation number: 9 (block: 8463761)
   > confirmation number: 10 (block: 8463762)

   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0x67ac2b0150a58a75122030575a97ae1688b38ee52c377761dc87c83da341ea89
   > Blocks: 0            Seconds: 20
   > contract address:    0xa220bD5718FC15fd83E1E1d5382d4249D37B57E2
   > block number:        8463763
   > block timestamp:     1675971444
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.139937652582987064
   > gas used:            312078 (0x4c30e)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002610060822461586 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463764)
   > confirmation number: 2 (block: 8463765)
   > confirmation number: 3 (block: 8463766)
   > confirmation number: 4 (block: 8463767)
   > confirmation number: 5 (block: 8463768)
   > confirmation number: 6 (block: 8463769)
   > confirmation number: 7 (block: 8463770)
   > confirmation number: 8 (block: 8463771)
   > confirmation number: 9 (block: 8463772)
   > confirmation number: 10 (block: 8463773)

   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0xa2777d7056165039b89c3547734764ae9d2c2ae5709daf46bb20316247d9ffd2
   > Blocks: 1            Seconds: 16
   > contract address:    0x70F1258825AA65eEBcBf9F19271890FB41CEE99e
   > block number:        8463775
   > block timestamp:     1675971660
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.137327591760525478
   > gas used:            312078 (0x4c30e)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002610060822461586 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463776)
   > confirmation number: 2 (block: 8463777)
   > confirmation number: 3 (block: 8463778)
   > confirmation number: 4 (block: 8463779)
   > confirmation number: 5 (block: 8463780)
   > confirmation number: 6 (block: 8463781)
   > confirmation number: 7 (block: 8463782)
   > confirmation number: 8 (block: 8463783)
   > confirmation number: 9 (block: 8463784)
   > confirmation number: 10 (block: 8463785)

   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0x345260b271f46a99b22dd07e3dc4584e3898d6afc91141968c9efa9286445288
   > Blocks: 1            Seconds: 20
   > contract address:    0x4139C73F1B7a0469B9bF5B9be95192b9184241DB
   > block number:        8463787
   > block timestamp:     1675971828
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.111983820717662309
   > gas used:            3030287 (0x2e3d0f)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.025343771042863169 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463788)
   > confirmation number: 2 (block: 8463789)
   > confirmation number: 3 (block: 8463790)
   > confirmation number: 4 (block: 8463791)
   > confirmation number: 5 (block: 8463792)
   > confirmation number: 6 (block: 8463793)
   > confirmation number: 7 (block: 8463794)
   > confirmation number: 8 (block: 8463795)
   > confirmation number: 9 (block: 8463796)
   > confirmation number: 10 (block: 8463797)
   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.035738801312867591 ETH

Summary
=======
> Total deployments:   6
> Final cost:          0.03763344094955451 ETH

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

•	https://goerli.etherscan.io/address/0x4139C73F1B7a0469B9bF5B9be95192b9184241DB

•	Contract: 0x4139C73F1B7a0469B9bF5B9be95192b9184241DB


Task 4: The application was successfully invoked to perform certain functions.

Account set up in Metamask using mnemonic provided (I had collected GoerliETH for this project using testnet faucets and distributed across the accounts for using it.) 

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/images/AccountSetup.png

Task 5: The application was successfully invoked and started.

Running command npm run dev invokes the coffee app and it is connected to owner account for ETH transactions.

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/images/UIview.png

Task 6: Transactions tested.



