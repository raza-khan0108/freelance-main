### Freelance ICP Platform (Deployed on ICP Mainnet)

This project is a fully decentralized freelance job board powered by the Internet Computer (ICP). It allows:

-  Clients to post jobs
-  Freelancers to send proposals
-  In-app chatting once a proposal is accepted

### 🔗 Live Mainnet App
👉 [Visit the App](https://k5ywt-3iaaa-aaaam-aelra-cai.icp0.io)

### ⚙️ Built With
- Internet Computer Protocol (ICP)
- Rust (backend)
- DFX SDK
- Candid Interface
- Vite + TypeScript (frontend)
  
---
### Clone & Run Locally

## Prerequisites

Ensure the following are installed:

- [Node.js & NPM](https://nodejs.org/)
- [Rust](https://www.rust-lang.org/tools/install)
- [DFX SDK](https://internetcomputer.org/docs/current/developer-docs/setup/install/)
- WASM target: bash
  rustup target add wasm32-unknown-unknown

  ### Steps to Clone and Deploy Locally
  
# Step 1: Clone the repository
git clone https://github.com/your_username/freelance-mainnet-deployment.git
cd freelance-mainnet-deployment

# Step 2: Install frontend dependencies
npm install

# Step 3: Start the local replica
dfx start --background

# Step 4: Deploy to local ICP replica
dfx deploy

# Access the frontend:
echo "http://localhost:4943/?canisterId=$(dfx canister id freelance_frontend)"

### Deploy to Mainnet

# Use your mainnet identity
dfx identity use freelance_mainnet

# Redeem your faucet coupon (only once)
dfx cycles redeem-faucet-coupon YOUR-COUPON-CODE --ic

# Deploy to mainnet
dfx deploy --ic


