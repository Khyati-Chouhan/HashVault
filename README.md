# HashVault 

**HashVault** is a secure decentralized file-sharing platform that combines blockchain-based ownership verification with robust client-side encryption. It ensures files remain fully private and accessible only to verified owners through MetaMask authentication. The system is powered by smart contracts that handle ownership records, access control, and role-based permissions, providing transparent, tamper-proof management of shared data.

 ## Project Overview

In an era where data breaches and unauthorized access are increasingly common, ensuring secure and verifiable data sharing is critical.
HashVault addresses this by leveraging blockchain technology to achieve decentralized ownership control and end-to-end encryption.

## Core Features

- Blockchain-based Ownership: Smart contracts store file hashes and access permissions immutably.
- Client-Side Encryption: Files are encrypted in the browser before upload—no plaintext ever leaves the client.
- MetaMask Integration: Wallet-based login for owner-only access and verification.
- Smart Contracts: Manage ownership transfer, access rights, and permission roles.
- Minimalistic UI: Clean, responsive interface for easy upload, share, and access workflows.
- Verifiable Proofs: On-chain verification ensures authenticity and ownership integrity.

 ## Tech Stack

- Frontend: React.js, TailwindCSS
- Blockchain: Solidity, Hardhat
- Wallet & Web3: MetaMask, Ethers.js
- Storage: IPFS / Pinata
- Backend: Node.js (optional metadata API)

## How to Setup (Locally)
Clone the Repository
```bash
git clone https://github.com/Khyati-Chouhan/HashVault.git
cd HashVault
```
Install Dependencies
```bash
npm install
```
Start Development Server
```bash
npm run dev
```
Build for Production
```bash
npm run build
```

## Deployment

Deploy easily on [Vercel](https://vercel.com), [Netlify](https://www.netlify.com), or [Render](https://render.com) for production use.  
You can also deploy the smart contract on any Ethereum testnet (e.g., Sepolia, Goerli) using Hardhat.

## Smart Contract Deployment (Hardhat)
```bash
npx hardhat compile
npx hardhat run scripts/deploy.js --network sepolia
