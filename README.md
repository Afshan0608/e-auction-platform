# Blockchain-Based E-Auction Platform



## Project Overview

This is a decentralized **E-Auction Platform** built on Ethereum blockchain technologies. It allows sellers to list products for auction and bidders to place bids securely through smart contracts. The platform uses **Ganache** as a local Ethereum blockchain simulator, **Metamask** as a wallet for managing crypto accounts, and **Flask** as the web interface backend framework.

---

## Features

### Seller Functionalities
- **Seller Signup:** Register as a seller by providing personal details and verification information.
- **Seller Signin:** Secure login for sellers.
- **Add Product:** Sellers can list their products/items for auction with details such as description, images, and starting price.
- **Check Status:** Sellers can monitor ongoing auctions, current highest bids, and auction end times.
- **Sell Product:** After an auction ends, ownership transfers from seller to winning bidder and transaction finalization is handled.

### Bidder Functionalities
- **Bidder Signup:** Register as a bidder with necessary personal info.
- **Bidder Signin:** Secure login for bidders.
- **Bid on Products:** Bidders can place bids on listed products.
- **View Bidder:** Sellers and admins can view bidder profiles and bidding history to evaluate credibility.

### Admin Functionalities
- **Admin Login:** Secure admin access.
- **View Transactions:** Admin can review all auction-related transactions between buyers, sellers, and the system.
- **View Seller Details:** Admin can view and manage seller profiles.
- **View Bidder Details:** Admin can view bidder profiles and activities.

---

## Technology Stack

| Component         | Technology                  |
|-------------------|-----------------------------|
| Blockchain        | Ethereum (Ganache for local simulation) |
| Smart Contracts   | Solidity                    |
| Wallet            | Metamask                   |
| Backend & UI      | Python Flask               |
| Database          | (Specify if used, else blockchain state) |
| Frontend          | Flask Templates (HTML, CSS, JS) |

---

## How It Works

1. Sellers register and list products for auction on the platform.
2. Bidders register and place bids on active auctions.
3. Smart contracts on the Ethereum blockchain manage bids, maintain auction states, and finalize transactions automatically.
4. Ganache simulates the Ethereum blockchain locally, while Metamask manages user wallets and transaction signing.
5. Flask provides the user interface, making interaction with blockchain seamless.

---

## Setup and Installation

### Prerequisites
- Python 3.x
- Node.js and npm
- Ganache (https://trufflesuite.com/ganache/)
- Metamask browser extension (Chrome or Firefox)
- Solidity compiler (via Truffle or Remix)
- Git

### Clone the Repository

git clone https://github.com/Afshan0608/e-auction-platform.git
cd e-auction-platform

### Python Virtual Environment and Dependencies
python3 -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt

### Start Ganache
Open Ganache and start a new workspace.

Note the RPC server address (usually http://127.0.0.1:7545).

### Configure Metamask
Install Metamask browser extension.

Connect Metamask to the Ganache local network using the RPC address.

Import Ganache accounts into Metamask using private keys shown in Ganache.

### Run the Flask Application

export FLASK_APP=app.py       # On Windows: set FLASK_APP=app.py
export FLASK_ENV=development  # Optional: for debug mode
flask run --host=0.0.0.0 --port=5000

### Access the Platform
Open your browser and go to http://localhost:5000.

Register as seller or bidder and interact with the auctions.

### How to Use the Platform
Seller: Sign up → Log in → Add products → Monitor auction status → Complete sales.

Bidder: Sign up → Log in → Browse auctions → Place bids → View auction results.

Admin: Log in → Manage users and transactions → Monitor platform activity.

### Future Enhancements
Deploy smart contracts on Ethereum public testnets (Sepolia, Goerli) instead of Ganache.

Implement payment gateway integration for real transactions.

Add notifications for bidders and sellers.

Improve UI/UX with React or Vue.js frontend.

Integrate decentralized storage (IPFS) for product images.


### Contact
Created by Afshan.
Feel free to open issues or pull requests for improvements.
