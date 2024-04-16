# FxPortal-Bridge

## NFT Collection Project 

## Overview
This project demonstrates the end-to-end process of creating a digital art NFT collection, from generation using AI through DALL-E 2 or Midjourney, to deployment on the Ethereum blockchain, and finally cross-chain bridging to the Polygon network. The repository includes scripts for generating art, minting tokens, and bridging these NFTs using a testnet environment.

### Components:
- **AI Art Generation:** Generate digital artworks using DALL-E 2 or Midjourney based on provided prompts.
- **Storage:** Upload and pin generated images on IPFS using Pinata.
- **Smart Contract:** Deploy an ERC721 or ERC1155 smart contract on the Ethereum testnet with additional features.
- **Cross-chain Mapping:** Utilize Polygon's network token mapping for visualization of the NFTs.
- **Automation Scripts:** Hardhat scripts for batch minting and transferring NFTs across blockchains.

## Prerequisites
- Node.js and npm
- Hardhat
- Ethereum wallet with Goerli testnet ETH
- Polygon wallet with Mumbai testnet MATIC
- Pinata.cloud account
- Access to DALL-E 2 or Midjourney

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourgithub/nft-collection-project.git
   cd nft-collection-project
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Set up Environment Variables**
   Create a `.env` file in the root directory and update it with your credentials:
   ```plaintext
   PRIVATE_KEY=your_private_key
   ALCHEMY_API_KEY=your_alchemy_api_key
   PINATA_API_KEY=your_pinata_api_key
   PINATA_SECRET_API_KEY=your_pinata_secret_api_key
   ```

## Usage

### Step 1: Generate Artwork
### Step 2: Deploy Smart Contract
- **Compile Contracts**
  ```bash
  npx hardhat compile
  ```
- **Deploy to Goerli**
  ```bash
  npx hardhat run scripts/deploy.js --network sepolia
  ```
  This will deploy your ERC721 or ERC1155 smart contract to the Goerli testnet.

### Step 3: Mint NFTs
- **Batch Mint using Hardhat Script**
  ```bash
  npx hardhat run scripts/mintNFTs.js --network sepolia
  ```

### Step 4: Transfer NFTs to Polygon Mumbai
- **Approve and Deposit NFTs**
### Step 5: Verify on Mumbai

## Additional Information

- **Smart Contract Features**
  The deployed smart contract includes a `promptDescription` function that returns the AI generation prompt used for each NFT image.

- **Cross-chain Functionality**
  The project demonstrates the use of the FxPortal bridge for transferring NFTs from Ethereum's testnet to Polygon's Mumbai testnet.

## Contributing
Contributions are welcome! Please feel free to submit any issues or pull requests.

## License
Distributed under the MIT License. See `LICENSE` for more information.

---

This README provides a basic template and workflow for a typical NFT project on GitHub. It can be further customized based on the specifics of your project and additional functionalities you might implement.
