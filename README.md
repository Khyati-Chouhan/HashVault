# SnapBlocks: Decentralized File Sharing App

SnapBlocks is a decentralized file-sharing platform designed to provide secure and decentralized storage using Ethereum smart contracts and IPFS. It ensures data integrity, ownership control, and efficient blockchain interactions.

## Features

- Decentralized file uploads using IPFS and Pinata API.  
- Blockchain-based access control and ownership management.  
- File retrieval via IPFS hashes stored on the Ethereum blockchain.  
- MetaMask integration for secure blockchain interactions.

## Tools and Technologies

- **Frontend**: ReactJS  
- **Blockchain**: Solidity and Hardhat  
- **Storage**: IPFS (managed via Pinata API)  
- **Authentication**: MetaMask  

## Setup Guide

### Prerequisites

Ensure you have the following installed:

- Node.js (v14 or later)  
- MetaMask browser extension  
- Pinata API Key and Secret Key  

### Installation Steps

1. Clone the repository:  
   ```bash
   git clone https://github.com/Alishba-Malik/CS360-semester-project/
   cd SnapBlocks
   ```

2. Install dependencies:  
   ```bash
   npm install
   ```

3. Initialize Hardhat:  
   ```bash
   npm install --save-dev hardhat
   npx hardhat init
   ```

## Configuration

1. **Smart Contract Address**:  
   Update the contract address in `src/App.jsx` after deployment.  

2. **Pinata API Keys**:  
   Add your Pinata API Key and Secret Key in `src/components/FileUpload.jsx` under the variables `pinata_api_key` and `pinata_secret_api_key`.  

## Running SnapBlocks

1. Start a local blockchain:  
   ```bash
   npx hardhat node
   ```

2. Deploy the smart contract in a new terminal:  
   ```bash
   npx hardhat run --network localhost scripts/deploy.js
   ```

3. Start the frontend in a new terminal:  
   ```bash
   cd SnapBlocks  
   npm run dev
   ```

4. Open your browser and navigate to [http://localhost:3000](http://localhost:3000).

## Security Considerations

- Implement encryption for sensitive files before uploading them to IPFS.  
- Ensure smart contracts have access controls to prevent unauthorized operations.

