# Minimal NFT Marketplace

A streamlined, secure, and expert-level NFT Marketplace contract. This repository provides the core logic for a decentralized exchange (DEX) specifically for NFTs.

### Key Logic
* **Listing:** Users can list their NFTs by providing the contract address, Token ID, and price.
* **Buying:** Users can purchase listed NFTs by sending the exact amount of Ether.
* **Escrow-less:** This contract uses the "Pull over Push" pattern and requires users to approve the marketplace, keeping the NFT in the user's wallet until the moment of sale.
* **Security:** Includes Reentrancy guards and ownership checks.

### Setup
1. Install dependencies (OpenZeppelin).
2. Compile using Hardhat or Foundry.
3. Deploy the `NftMarketplace.sol` contract.

### Gas Optimization
This contract uses `error` types instead of `require` strings to save significant gas during deployment and execution.
