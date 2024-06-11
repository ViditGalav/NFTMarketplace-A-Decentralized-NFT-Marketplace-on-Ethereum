NFTMarketplace: A Decentralized NFT Marketplace on Ethereum


This full-stack project demonstrates a decentralized marketplace for buying and selling NFTs (Non-Fungible Tokens) on the Ethereum blockchain. It leverages smart contracts for secure transactions and provides a user-friendly interface for interacting with the marketplace.

Key Features
NFT Creation and Listing: Users can create and list their own NFTs for sale.
Browsing and Purchasing: Browse available NFTs and purchase them directly with ETH (Ethereum's native cryptocurrency).
Ownership Tracking: Securely tracks ownership of NFTs on the blockchain.
Listing Fee: A small fee is charged to list NFTs, providing a revenue stream for the marketplace owner.
Upgradeable Listing Price: The marketplace owner can adjust the listing fee.
Technical Overview
Blockchain: Ethereum (Chosen for its established NFT standards, smart contract capabilities, and decentralized nature)
Smart Contracts:
Language: Solidity (^0.8.0)
Libraries: OpenZeppelin (for secure ERC-721 token implementation and Counters utility)
Core Functions:
createToken(string memory tokenURI, uint256 price): Creates and lists a new NFT.
getAllNFTs(): Retrieves all listed NFTs.
getMyNFTs(): Fetches NFTs owned or listed by the current user.
executeSale(uint256 tokenId): Completes the purchase of an NFT.
updateListPrice(uint256 _listPrice): Updates the listing fee (owner only).


Frontend:
Framework: React (for building the user interface)
Components:
Navbar.js: Navigation bar for the application.
NFTTile.js: Displays individual NFT listings.
Marketplace.js: The main marketplace page showing listed NFTs.
Profile.js: User profile page to view owned NFTs.
SellNFT.js: Form for creating and listing new NFTs.
External Libraries:
Axios (for making HTTP requests)
ethers.js (for interacting with Ethereum and smart contracts)
Pinata (for storing NFT metadata and images on IPFS)


Getting Started
Prerequisites:
MetaMask: Install and configure MetaMask to interact with the Ethereum blockchain.
Node.js and npm: Ensure Node.js and npm are installed.
Pinata Account: Create an account on Pinata to store NFT data.
