# 🏠 RentalChain DApp - Remix Edition

**Polygon Amoy Testnet | Chain ID: 80002**

---

## 📌 Project Overview
RentalChain is a decentralized application (DApp) that enables secure rental agreement creation, signing, and verification using blockchain technology.  
It leverages smart contracts, IPFS storage, and MetaMask wallet integration.

---

## 📁 Project Structure
```
contract/
└── RentalAgreement.sol # Smart contract for deployment in Remix

frontend/
├── src/
│ ├── utils/contract.ts # Blockchain interaction logic
│ └── hooks/useWallet.ts # Wallet connection & state management
└── ... # React + Vite frontend
```

---

## 🚀 Quick Setup

### 🔹 1) Deploy Contract in Remix
1. Open https://remix.ethereum.org  
2. Create file: `contracts/RentalAgreement.sol`  
3. Paste contract code from `contract/RentalAgreement.sol`  
4. Compile using **Solidity 0.8.19**  
5. Go to **Deploy & Run Transactions**  
6. Select **Injected Provider - MetaMask**  
7. Ensure MetaMask is connected to **Polygon Amoy (Chain ID 80002)**  
8. Click **Deploy** and confirm transaction  
9. Copy the deployed **contract address**  

---

### 🔹 2) Configure Frontend Environment
Create a `.env` file inside `frontend/` and add:

```env
VITE_CONTRACT_ADDRESS=your_deployed_contract_address
VITE_PINATA_API_KEY=your_pinata_api_key
VITE_PINATA_SECRET_KEY=your_pinata_secret_key
```
### 🔹 3) Start Frontend
cd frontend
npm install
npm run dev
