# Onyx-SSI-Paymaster
This project demonstrates building a custom paymaster on zkSync Era, allowing users to pay transaction fees with any ERC20 token, integrated with a Dockerized zkSync node.

## Overview

- Implement a paymaster that uses ERC20 tokens for transaction fees.
- Realize the paymaster with a Dockerized zkSync node for enhanced compatibility and scalability.

## Prerequisites

- Node.js (version 16).
- Docker.
- Familiarity with zkSync and smart contract deployment.
- MetaMask wallet.

## Setup for Smart Contracts

1. **Clone the Repository**:
   ```bash
   git clone [repository-link]
   cd Paymaster-Dockerized
   ```

2. **Install Dependencies**:
    ```bash
    yarn
    ```

3. **Compile the Contracts:**:
    ```bash
    yarn hardhat compile
    ```
## Deploy Smart Contracts

1. **Set Up Dockerized zkSync Node**:
    ```bash
    npx zksync-cli dev start
    ```

2. **Deploy the Contracts**:
    ```bash
    yarn hardhat deploy-zksync --script deploy-greeter.ts
    ```

## Set the Frontend:

1. **Install Dependencies**:
    ```bash
    cd ../frontend
    yarn
    nvm install 16
    nvm use 16
    ```

2. **Spin up the Project**:
    ```bash
    yarn serve
    ```

## Troubleshooting
- Ensure the paymaster has sufficient ETH for transaction fees.
- If using older Node.js versions (like 16), the frontend may only be compatible with those.
- Ensure rich accounts have adequate tokens before transactions.

## Future Goals
Seamlessly integrate the custom paymaster with Onyx SSI, enhancing decentralized identity solutions.