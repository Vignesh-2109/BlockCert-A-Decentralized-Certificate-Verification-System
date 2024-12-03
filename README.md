# BlockCert - A Decentralized Certificate Verification System

[![Blockchain](https://img.shields.io/badge/Blockchain-Ethereum-brightgreen)](https://ethereum.org/)
[![IPFS](https://img.shields.io/badge/Storage-IPFS-blue)](https://ipfs.io/)
[![MetaMask](https://img.shields.io/badge/Wallet-MetaMask-orange)](https://metamask.io/)
[![Truffle](https://img.shields.io/badge/Framework-Truffle-yellowgreen)](https://trufflesuite.com/)

## Introduction

**BlockCert** is a blockchain-based certificate verification system that ensures the authenticity and integrity of certificates issued by educational institutions, employers, and other organizations. Built on the Ethereum blockchain and using decentralized storage via **IPFS**, this system provides a secure, transparent, and efficient solution for issuing, storing, and verifying certificates.

The project leverages **smart contracts** to automate the process, and **MetaMask** is used for secure login and digital signatures. It includes three main entities:
- **Student**: Receives certificates.
- **Institute**: Issues certificates to students.
- **Employer**: Verifies certificates issued by institutes.

## Features

- 🚀 **Blockchain-based Verification**: Ensures that certificates cannot be altered once issued.
- 🔐 **Secure Login with MetaMask**: Uses MetaMask for user authentication and signing transactions.
- 🌐 **Decentralized Storage with IPFS**: Certificates are stored securely on IPFS with content references stored on the blockchain.
- 📜 **Smart Contracts**: Automates certificate issuance and verification processes.
- 🔍 **Transparency**: Provides full transparency and auditability of all issued certificates.

## Technology Stack

- **Ethereum**: Blockchain platform for immutability and security.
- **IPFS**: Decentralized file storage for certificate PDFs.
- **MetaMask**: Ethereum wallet for user authentication and signing transactions.
- **Truffle Suite**: For smart contract development and deployment.
- **Ganache CLI**: Local Ethereum blockchain for development.
- **Streamlit**: Python library for creating web applications and user interfaces.
- **Docker**: Containerizes the entire application for easy deployment.

## Installation

### Prerequisites

Make sure you have the following installed:

- **Node.js (v21.0.0 or higher)**: [Download Node.js](https://nodejs.org/)
- **Python (3.9.10 or higher)**: [Download Python](https://www.python.org/downloads/)
- **Docker**: [Download Docker](https://www.docker.com/get-started)
- **Ganache CLI**: Install Ganache for running a local Ethereum blockchain:
  ```bash
  npm install -g ganache-cli

Truffle: Install Truffle for smart contract development:
npm install -g truffle
Installation Steps
Clone the Repository:

bash
Copy code
git clone https://github.com/Vignesh-2109/BlockCert-A-Decentralized-Certificate-Verification-System.git
Install Dependencies:

bash
Copy code
cd BlockCert-A-Decentralized-Certificate-Verification-System
npm install
Setup Ganache:

Start Ganache CLI in a separate terminal window to run a local Ethereum blockchain.
bash
Copy code
ganache-cli
Deploy Smart Contracts:

Navigate to the Truffle directory and deploy the smart contracts to your local blockchain.
bash
Copy code
truffle migrate
Run the Web Application:

Start the Streamlit app to open the frontend application in your browser.
bash
Copy code
streamlit run app.py
Access the DApp:

Open your browser and go to http://localhost:8501 to access the certificate verification system.
Usage
Institutes can log in via MetaMask, input student details, and issue certificates.
Students can retrieve their certificates and provide them to Employers for verification.
Employers can verify certificates by entering the Certificate ID or uploading the certificate file.
Verification results will confirm if the certificate is authentic or tampered with.
Workflow
1. Certificate Issuance Process:
The institute logs in using MetaMask.
The institute inputs the certificate details.
A unique Certificate ID (CID) is generated, and the certificate's data is hashed.
The hash is signed with the issuer’s private key, and the signed certificate is stored on the blockchain.
The certificate PDF is uploaded to IPFS, and the CID of the PDF is stored on the blockchain.
2. Certificate Verification Process:
Employers log in using MetaMask.
Employers can either input the Certificate ID or upload the certificate PDF.
The certificate details and hash are retrieved from the blockchain.
The hash of the uploaded certificate is recalculated and compared with the one stored on the blockchain.
If the hashes match, the certificate is valid; otherwise, it is flagged as invalid.
Contributing
We welcome contributions from the community! To contribute to this project:

Fork the repository.
Create a new branch for your feature or fix.
Commit your changes and push to your branch.
Submit a pull request to the main repository.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Ethereum for providing the decentralized platform for secure, transparent transactions.
IPFS for enabling decentralized storage and efficient file retrieval.
MetaMask for secure login and transaction signing.
Truffle for simplifying smart contract development and deployment.
Streamlit for building the frontend web application.
Ganache CLI for running a local Ethereum blockchain for development and testing.

