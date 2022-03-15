# Udacity Blockchain Capstone

This project is about creating a marketplace for real estate in the Ethereum blockchain. Each property is represented by ERC721 token.
Zk-Snark is used to prove that you have the title deed of the property without sharing specific information about the property.
After verification by Zk-Snark, the token is listed in a market place - OpenSea for sale.

# Install > Test > Deploy

1. Clone this repository git clone https://github.com/bamsby/Blockchain-Capstone.git
2. Install dependencies npm install and npm install --save truffle-hdwallet-provider
3. Start Ganache by typing ganache-cli -a 40 -m "candy maple cake sugar pudding cream honey rich smooth crumble sweet treat"
4. Open a separate terminal, cd into eth-contracts and compile by typing truffle compile
5. Run test by typing the following:
   a. truffle test test/TestERC721Mintable.js
   b. truffle test test/TestSquareVerifier.js
   c. truffle test test/TestSolnSquareVerifier.js
6. Check that all the tests passed.
7. Migrate to rinkeby by typing truffle migrate --network rinkeby

# Contract Info

## Address

0x8cdaf0cd259887258bc13a92c0a6da92698644c0

## ABI

[ { constant: true,
inputs: [ [Object] ],
name: 'supportsInterface',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: true,
inputs: [ [Object] ],
name: 'getApproved',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object] ],
name: 'approve',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: true,
inputs: [],
name: 'getSymbol',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object] ],
name: 'setPaused',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: true,
inputs: [],
name: 'getName',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: true,
inputs: [],
name: 'totalSupply',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object], [Object] ],
name: 'transferFrom',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object] ],
name: '**callback',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: true,
inputs: [ [Object], [Object] ],
name: 'tokenOfOwnerByIndex',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object], [Object] ],
name: '**callback',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object], [Object] ],
name: 'safeTransferFrom',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: true,
inputs: [ [Object] ],
name: 'tokenByIndex',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object], [Object], [Object] ],
name: 'verifyTx',
outputs: [ [Object] ],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: true,
inputs: [ [Object] ],
name: 'ownerOf',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: true,
inputs: [ [Object] ],
name: 'balanceOf',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: true,
inputs: [],
name: 'getOwner',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object] ],
name: 'setApprovalForAll',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object], [Object], [Object] ],
name: 'safeTransferFrom',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: true,
inputs: [],
name: 'getBaseTokenURI',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: true,
inputs: [ [Object] ],
name: 'tokenURI',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: true,
inputs: [ [Object], [Object] ],
name: 'isApprovedForAll',
outputs: [ [Object] ],
payable: false,
stateMutability: 'view',
type: 'function' },
{ constant: false,
inputs: [ [Object] ],
name: 'transferOwnership',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ anonymous: false,
inputs: [ [Object], [Object], [Object] ],
name: 'SolutionAdded',
type: 'event' },
{ anonymous: false,
inputs: [ [Object], [Object], [Object] ],
name: 'Transfer',
type: 'event' },
{ anonymous: false,
inputs: [ [Object], [Object], [Object] ],
name: 'Approval',
type: 'event' },
{ anonymous: false,
inputs: [ [Object], [Object], [Object] ],
name: 'ApprovalForAll',
type: 'event' },
{ anonymous: false,
inputs: [ [Object] ],
name: 'Paused',
type: 'event' },
{ anonymous: false,
inputs: [ [Object] ],
name: 'Unpaused',
type: 'event' },
{ anonymous: false,
inputs: [ [Object], [Object] ],
name: 'ownershipTransferred',
type: 'event' },
{ anonymous: false,
inputs: [ [Object] ],
name: 'Verified',
type: 'event' },
{ constant: false,
inputs:
[ [Object], [Object], [Object], [Object], [Object], [Object] ],
name: 'addSolution',
outputs: [],
payable: false,
stateMutability: 'nonpayable',
type: 'function' },
{ constant: false,
inputs: [ [Object], [Object] ],
name: 'mint',
outputs: [ [Object] ],
payable: false,
stateMutability: 'nonpayable',
type: 'function' } ]

# OpenSea Marketplace Link

https://testnets.opensea.io/collection/chrisbamsby-collection

# OpenSea Listings

https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015755882341597185/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015756981853224961/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015758081364852737/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015759180876480513/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015760280388108289/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015761379899736065/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015762479411363841/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015763578922991617/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015764678434619393/
https://testnets.opensea.io/assets/0x88b48f654c30e99bc2e4a1559b4dcf1ad93fa656/106503804230293455861048682397403735248937668577190190245642015765777946247169/

# Project Resources

- [Remix - Solidity IDE](https://remix.ethereum.org/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Truffle Framework](https://truffleframework.com/)
- [Ganache - One Click Blockchain](https://truffleframework.com/ganache)
- [Open Zeppelin ](https://openzeppelin.org/)
- [Interactive zero knowledge 3-colorability demonstration](http://web.mit.edu/~ezyang/Public/graph/svg.html)
- [Docker](https://docs.docker.com/install/)
- [ZoKrates](https://github.com/Zokrates/ZoKrates)
