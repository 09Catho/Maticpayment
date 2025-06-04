# Matic Payment Gateway for Byte Net

## Introduction

This repository contains the code for integrating a **Matic (Polygon)** payment gateway, designed to be used for secure and transparent transactions on the **Byte Net** platform. The gateway allows users to send Matic tokens to access premium content and resources on the platform. 

### Note: 
This payment gateway has not been integrated into our live website due to the lack of funds needed to rent a VPS (Virtual Private Server) for hosting the node server. However, the complete code is provided here, and anyone can use it to implement the Matic payment gateway by setting up their own server.

## How to Set Up and Run

### Prerequisites

- **Node.js**: Ensure you have the latest version of Node.js installed on your system.
- **Matic Wallet**: You'll need your Matic wallet details (private key and wallet address).
- **VPS Server**: Required to host the payment gateway if you plan to deploy it live.

### Steps to Run the Payment Gateway

1. **Download and Extract**
   - Clone the repository or download the zip file and extract it:
     ```bash
     git clone https://github.com/09Catho/Maticpayment.git
     ```
     OR download the zip and extract it manually.

2. **Navigate to the Project Directory**
   - Open a terminal and navigate to the extracted folder:
     ```bash
     cd Maticpayment
     ```

3. **Install Dependencies**
   - Run the following command to install the required dependencies:
     ```bash
     npm install
     ```

4. **Configure Your Wallet Details**
   - Inside the project directory, open the `server.js` file and replace the placeholder values with your **Matic wallet credentials**:
     ```javascript
     module.exports = {
       walletPrivateKey: "YOUR_PRIVATE_KEY",
       walletAddress: "YOUR_WALLET_ADDRESS",
       infuraEndpoint: "YOUR_INFURA_ENDPOINT",  // Or any other RPC provider for Matic
     };
     ```

5. **Start the Server**
   - Once everything is set up, you can start the server using the following command:
     ```bash
     node server.js
     ```
   - The server will begin listening for payment transactions made in Matic tokens.

### Deployment

- **VPS Hosting (Required for Live Implementation)**: To fully integrate this into your live platform, you will need a VPS (e.g., DigitalOcean, AWS, etc.) to host the payment gateway.
- Once the server is deployed on a VPS, users can securely make Matic transactions for VIP access on Byte Net.

## Why We Haven't Integrated This Feature Yet

At the moment, the Matic payment gateway isn't live on the Byte Net platform due to insufficient funds to rent a VPS server to host the node server. However, all the necessary code has been made available here, and you are free to use, modify, and deploy it according to your needs.

## Contributing

If you'd like to contribute to this project, feel free to submit pull requests or report any issues. We appreciate any feedback or improvements to the code.

1. Fork the repository  
2. Create your feature branch (`git checkout -b feature-name`)  
3. Commit your changes (`git commit -m "Add feature"`)  
4. Push to the branch (`git push origin feature-name`)  
5. Open a pull request  

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Creators

This project was developed with love and technical enthusiasm by:

### 👨‍💻 Atul  
### 👩‍💻 Divyanshi Sharma  

Together, they envisioned a seamless blockchain-based payment system to power decentralized access to digital content on Byte Net. Their contribution to open-source development aims to help others build secure Web3 solutions with ease.

---

Thank you for exploring the Matic Payment Gateway for Byte Net! We hope this resource helps you implement secure blockchain payments for your platform.
