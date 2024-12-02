# ETH + AVAX Proof: Intermediate EVM Course Assessment - Smart Contract Management

This Solidity program is part of the assessment for the Metacrafter's ETH + AVAX Proof: Intermediate EVM Course. The purpose of this project is to create a simple smart contract with basic functionalities and display the values of its functions in a frontend application.

## Description

The contract allows the owner to interact with basic functions such as depositing, withdrawing funds, and updating a stored message. The frontend provides a user-friendly interface to interact with these contract functions.

### Contract Features:
- **Get Balance:** Retrieve the contract's balance.
- **Get Message:** Retrieve the current stored message.
- **Set Message:** Update the message (only allowed by the owner).
- **Deposit:** Deposit ETH into the contract (only allowed by the owner).
- **Withdraw:** Withdraw ETH from the contract (only allowed by the owner).

## Getting Started

Follow the steps below to get the project running on your local machine.

### Prerequisites

Ensure that you have the following installed:
- **Node.js**: [Download Node.js](https://nodejs.org/)
- **MetaMask**: [Install MetaMask](https://metamask.io/)

### Installation Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/AngeloCoder27/ETHAVAX-PROOF-Intermediate-EVM-Course2.git
   cd ETHAVAX-PROOF-Intermediate-EVM-Course2
   ```

2. Install the required dependencies:
   ```bash
   npm install
   ```

3. Open two additional terminals in your VS code:
   - In the second terminal, start a local Hardhat node:
     ```bash
     npx hardhat node
     ```

   - In the third terminal, deploy the contract to the local node:
     ```bash
     npx hardhat run --network localhost scripts/deploy.js
     ```

4. Back in the first terminal, start the frontend development server:
   ```bash
   npm run dev
   ```

   The frontend will be running on [http://localhost:3000/](http://localhost:3000/).

### Using the Application

1. **Connect MetaMask**: Connect your MetaMask wallet to interact with the smart contract.

2. **Interact with the Contract**: 
   - You can **set the message** using the "Set Message" button.
   - **Deposit 1 ETH** or **Withdraw 0.5 ETH** using the corresponding buttons.

   The contract balance and stored message will be displayed, and you can interact with the contract functions through the interface.

### Contract Functions

- **getBalance()**: Returns the current balance of the contract.
- **getMessage()**: Returns the current message stored in the contract.
- **setMessage(string newMessage)**: Allows the owner to change the message stored in the contract.
- **deposit(uint256 _amount)**: Allows the owner to deposit ETH into the contract.
- **withdraw(uint256 _withdrawAmount)**: Allows the owner to withdraw ETH from the contract.

## Authors
- @AngeloCoder27

Based on the SCM-Starter Template from: [@MetacrafterChris](https://github.com/MetacrafterChris)
