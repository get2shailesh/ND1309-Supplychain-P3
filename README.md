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

   Replacing 'Migrations'
   ----------------------
   > transaction hash:    0xc9289ff6aa22e821d301da41dc9365c87248ecfc058bf745d321a642f4c77267
   > Blocks: 0            Seconds: 20
   > contract address:    0x72121b2173Ade3eA87CA7473DcBc8D22B180C0BB
   > block number:        8463368
   > block timestamp:     1675965612
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.157114589240602222
   > gas used:            226537 (0x374e9)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.001894639636686919 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463369)
   > confirmation number: 2 (block: 8463370)
   > confirmation number: 3 (block: 8463371)
   > confirmation number: 4 (block: 8463372)
   > confirmation number: 5 (block: 8463373)
   > confirmation number: 6 (block: 8463374)
   > confirmation number: 7 (block: 8463375)
   > confirmation number: 8 (block: 8463376)
   > confirmation number: 9 (block: 8463377)
   > confirmation number: 10 (block: 8463378)
   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.001894639636686919 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0xdce571c9075ad81eb8e10b08ff0804929b67c19056b6fb529dd64310a81471f1
   > Blocks: 1            Seconds: 12
   > contract address:    0xe43333E63e8A856bb3e23CB8b3238eF0e2C0938D
   > block number:        8463380
   > block timestamp:     1675965792
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.154166902743335133
   > gas used:            306684 (0x4adfc)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002564948164483908 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463381)
   > confirmation number: 2 (block: 8463382)
   > confirmation number: 3 (block: 8463383)
   > confirmation number: 4 (block: 8463384)
   > confirmation number: 5 (block: 8463385)
   > confirmation number: 6 (block: 8463386)
   > confirmation number: 7 (block: 8463387)
   > confirmation number: 8 (block: 8463388)
   > confirmation number: 9 (block: 8463389)
   > confirmation number: 10 (block: 8463390)

   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x418a2b02323802520ebe09761bd7d99ae789ce23c79533b88a76252fb84a3e01
   > Blocks: 0            Seconds: 8
   > contract address:    0x467B6CC911D854c712c2c9e129EFf5374e03094b
   > block number:        8463391
   > block timestamp:     1675965924
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.151556942282737791
   > gas used:            312066 (0x4c302)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002609960460597342 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463392)
   > confirmation number: 2 (block: 8463393)
   > confirmation number: 3 (block: 8463394)
   > confirmation number: 4 (block: 8463395)
   > confirmation number: 5 (block: 8463396)
   > confirmation number: 6 (block: 8463397)
   > confirmation number: 7 (block: 8463398)
   > confirmation number: 8 (block: 8463399)
   > confirmation number: 9 (block: 8463400)
   > confirmation number: 10 (block: 8463401)

   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0x191a93afe5ea331b403047e9243ac7cfba5f9b73c71ee85a2b904c335ceca5d0
   > Blocks: 1            Seconds: 24
   > contract address:    0x094afEbCd206B5C956557d0C1c336A8B7250EEa4
   > block number:        8463402
   > block timestamp:     1675966092
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.148946881460276205
   > gas used:            312078 (0x4c30e)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002610060822461586 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463403)
   > confirmation number: 2 (block: 8463404)
   > confirmation number: 3 (block: 8463405)
   > confirmation number: 4 (block: 8463406)
   > confirmation number: 5 (block: 8463407)
   > confirmation number: 6 (block: 8463408)
   > confirmation number: 7 (block: 8463409)
   > confirmation number: 8 (block: 8463410)
   > confirmation number: 9 (block: 8463411)
   > confirmation number: 10 (block: 8463412)

   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x9d1ef453d1ccb887f2a7d511b2802e0a6b9bfb6550b91e50921b07e75f7f0faa
   > Blocks: 0            Seconds: 8
   > contract address:    0x107fE93F45b2d56Ec722577f337829259fe19f99
   > block number:        8463413
   > block timestamp:     1675966236
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.146336820637814619
   > gas used:            312078 (0x4c30e)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.002610060822461586 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463414)
   > confirmation number: 2 (block: 8463415)
   > confirmation number: 3 (block: 8463416)
   > confirmation number: 4 (block: 8463417)
   > confirmation number: 5 (block: 8463418)
   > confirmation number: 6 (block: 8463419)
   > confirmation number: 7 (block: 8463420)
   > confirmation number: 8 (block: 8463421)
   > confirmation number: 9 (block: 8463422)
   > confirmation number: 10 (block: 8463423)

   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0x2eb0984e33a1cfcb9668b046df0a806e8f7c4e6c5ab8ebdf8440db129cb851d0
   > Blocks: 1            Seconds: 12
   > contract address:    0x1133717762e240e1282CD4a2027bFd6e1b144389
   > block number:        8463424
   > block timestamp:     1675966404
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             0.12099304959495145
   > gas used:            3030287 (0x2e3d0f)
   > gas price:           8.363488687 gwei
   > value sent:          0 ETH
   > total cost:          0.025343771042863169 ETH

   Pausing for 10 confirmations...

   --------------------------------
   > confirmation number: 1 (block: 8463425)
   > confirmation number: 2 (block: 8463426)
   > confirmation number: 3 (block: 8463427)
   > confirmation number: 4 (block: 8463428)
   > confirmation number: 5 (block: 8463429)
   > confirmation number: 6 (block: 8463430)
   > confirmation number: 7 (block: 8463431)
   > confirmation number: 8 (block: 8463432)
   > confirmation number: 9 (block: 8463433)
   > confirmation number: 10 (block: 8463434)
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

•	https://goerli.etherscan.io/address/0x1133717762e240e1282CD4a2027bFd6e1b144389

•	Contract: 0x1133717762e240e1282CD4a2027bFd6e1b144389

[The following details are from the initial contract deployment for initial submission, as per the feedback, I have re-deployed the contract]

•	Initial “Contract Address” on the Goerli Network:
For second review:
https://goerli.etherscan.io/address/0x8c7E1c25df2e4f51d8A8F5b4c1888401C33A2F60
For first review:
https://goerli.etherscan.io/address/0xFB1e9CF1D94fb443a07aA84DB5FAd869784dCa55

•	Initial Contract for reference: 
For second review:
0x8c7E1c25df2e4f51d8A8F5b4c1888401C33A2F60
For first review:
0xFB1e9CF1D94fb443a07aA84DB5FAd869784dCa55]

Task 4: The application was successfully invoked to perform certain functions.

Account set up in Metamask using mnemonic provided (I had collected GoerliETH for this project using testnet faucets and distributed across the accounts for using it.) 

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/images/AccountSetup.png

Task 5: The application was successfully invoked and started.

Running command npm run dev invokes the coffee app and it is connected to owner account for ETH transactions.

https://github.com/get2shailesh/ND1309-Supplychain-P3/blob/main/images/UIview.png

Task 6: Transactions tested.



