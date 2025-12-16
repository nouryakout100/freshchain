# FreshChain – Project Report

🔗 **Project Link:**  
https://nouryakout100.github.io/freshchain/

---

## Project Overview
FreshChain is a blockchain-based system for tracking food products across the supply chain.  
It records product data from production to retail using Ethereum smart contracts, ensuring transparency and data integrity.

---

## System Features
Each product batch stored on the blockchain includes:
- Product name and quantity  
- Ownership history  
- Sensor data (temperature, humidity, location)  
- Final inspection status (pass / fail)  

All recorded data is immutable.

---

## How the System Works
The system uses role-based access control.

### Admin
- Deploys the smart contract  
- Registers addresses for Producer, Transporter, Distributor, and Retailer  
- Only the admin can assign roles  

### Producer
- Creates a new batch with a unique ID  
- Enters product name and quantity  
- Example: Batch ID 1, Orange, Quantity 10  

### Transporter
- Adds temperature, humidity, and location data to the batch  

### Distributor
- Transfers batch ownership to the retailer  
- Only the current batch owner can transfer ownership  

### Retailer
- Performs final inspection  
- Marks the batch as approved or rejected  
- Requires switching to the retailer MetaMask account  

### Customer
- Generates a QR code linked to the batch  
- Views full product history in read-only mode  
- No MetaMask required  

---

## Technologies Used

### Blockchain
- Solidity  
- Ethereum (Sepolia Testnet)  
- Remix IDE  

### Frontend
- HTML, CSS, JavaScript  
- Ethers.js  
- MetaMask  
- QR Code API  
- GitHub Pages  

---

## Conclusion
FreshChain demonstrates how blockchain can improve food supply chain transparency.  
Authorized users can update data, while customers can verify product history using a QR code.
