# 🌾 AgriChain – Blockchain-based Agri Trading & Logistics Platform

### 🚀 Empowering Indian Farmers with Transparency, Traceability & Trust

---

## 📌 Table of Contents
- [About the Project](#about-the-project)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Modules](#modules)
- [Getting Started](#getting-started)
- [Folder Structure](#folder-structure)
- [Smart Contracts](#smart-contracts)
- [Mobile App](#mobile-app)
- [API Reference](#api-reference)
- [Contributing](#contributing)
- [License](#license)

---

## 🧭 About the Project

AgriChain is a blockchain-powered agricultural trading and logistics platform tailored for India’s farming ecosystem. It connects farmers, buyers, mandis, and transporters through a decentralized, secure, and traceable platform using smart contracts and mobile-first access.

---

## 💻 Tech Stack

- **Blockchain:** Hyperledger Fabric (Private Permissioned Ledger)
- **Frontend:** React Native (Mobile App)
- **Backend:** Node.js + Express.js
- **Database:** MongoDB / PostgreSQL
- **Smart Contracts:** Chaincode in Go
- **DevOps:** Docker, GitHub Actions, Nginx
- **Payments:** UPI (via Razorpay or Paytm)
- **IoT:** QR Tracking + GPS + Humidity sensors

---

## 🏗️ Architecture

```
Farmer App → Backend API → Blockchain (Fabric) → Buyer App / Mandi Dashboard
                      ↘ IoT Devices / QR Logs
                      ↘ UPI / Payment Gateway
```

---

## 📱 Modules

**1. Farmer App**  
- Crop Listing  
- Offers & Trade Contracts  
- Live Price Feed  
- Logistics Status  
- Wallet & Payments

**2. Admin Dashboard**  
- Verify Trades  
- Monitor Transactions  
- Manage Disputes  
- Analytics

**3. Blockchain Layer**  
- Smart Contracts: Trade, Logistics, Settlement  
- Identity Management: Farmer, Buyer, Transport  
- Event Logging and Audit Trail

---

## 🛠️ Getting Started

```bash
# Clone the repo
git clone https://github.com/AryanTanwar/Agi-Blockchain.git
cd Agi-Blockchain

# Install backend dependencies
cd backend
npm install

# Run backend
npm run dev

# Launch mobile app
cd ../mobile
npm install
npx react-native run-android
```

---

## 🗂️ Folder Structure

```
agrichain/
├── backend/
│   ├── controllers/
│   ├── routes/
│   └── smart-contracts/
├── mobile/
│   ├── screens/
│   ├── components/
├── fabric-network/
│   └── chaincode/
├── docs/
│   └── wireframes, flowcharts
```

---

## 🧠 Smart Contracts

- `CropTrade.go` – Handles trade offers and agreements  
- `Logistics.go` – Tracks shipments and updates QR-based logs  
- `Wallet.go` – Manages digital balance & UPI payouts  

Contracts use **Chaincode + CouchDB state database** and are deployed on Fabric peer nodes.

---

## 🔌 API Reference (Sample)

| Method | Route | Description |
|--------|-------|-------------|
| GET | /api/crops | Get all listed crops |
| POST | /api/trade/offer | Submit trade offer |
| POST | /api/logistics/update | Update shipment GPS & QR |
| POST | /api/payment/settle | Trigger payout |

---

## 🙌 Contributing

We welcome all contributors—developers, designers, agri experts, and blockchain enthusiasts!

```bash
# Fork the repo and create your branch
git checkout -b feature/your-feature

# Commit your changes
git commit -m "Add your feature"

# Push and create a PR
git push origin feature/your-feature
```

---

## 📜 License

This project is licensed under the MIT License. See `LICENSE` file for details.