🔍 AI Content Verification & Blockchain Audit Platform

An AI-powered platform for content authenticity analysis with cloud-based audit logging and blockchain verification.

This system helps verify the credibility of digital content such as:

News articles

Online publications

User-generated content

Social media posts

AI analyzes the credibility and authenticity of the content, while the results are stored in Cloud Storage and Blockchain to ensure transparency, traceability, and tamper-proof verification.

🌟 Key Features
🤖 AI Authenticity Scoring

The platform uses Google's Gemini 2.5 Flash model to analyze content and generate:

Confidence Score

AI Analysis Result

Structured JSON Output

This allows the system to evaluate the reliability of information automatically.

🧹 Data Cleansing Pipeline

The Node.js API layer handles data preprocessing before analysis:

Input Validation

Data Normalization

Structured JSON Transformation

This ensures the AI model receives clean and standardized input data.

☁️ Immutable Cloud Logging

All AI analysis results are securely stored in Amazon Web Services Amazon S3 to create a reliable audit trail.

Benefits include:

Historical verification capability

Protection against data tampering

Transparent audit records

⛓️ Blockchain Verification Registry

A Solidity Smart Contract is used to register verification results on blockchain.

The smart contract enables:

Verification record registration

Attestation storage

Content hash verification

This ensures that verification records are immutable, transparent, and publicly auditable.

⚙️ Operational Excellence

The system is designed to run in a production environment using:

Amazon Web Services Amazon EC2 (Amazon Linux)

Node.js Runtime

PM2 Process Manager

This architecture enables the service to run 24/7 with high reliability and scalability.

🧠 System Architecture
User / Dashboard
       │
       ▼
Frontend (React.js Dashboard)
       │
       ▼
Backend API (Node.js / Express)
       │
       ├── AI Analysis (Gemini API)
       │
       ├── Cloud Logging (AWS S3)
       │
       └── Blockchain Attestation
               │
               ▼
        Smart Contract (Solidity)
📂 Project Structure
ai-verificationAWS/
│
├── AIVerificationRegistryV2.sol
│   Smart Contract (Solidity)
│   Used for recording audit trails and verification attestations on blockchain
│
├── server.js
│   Backend API (Node.js / Express)
│   Handles AI analysis logic and integration with Cloud and Blockchain
│
├── abi.json
│   Application Binary Interface
│   Used for interacting with smart contract functions
│
├── dashboard/
│   React.js frontend dashboard
│
│   ├── src/
│   │   Main source code for UI components
│   │
│   └── public/
│       Static assets for web hosting
│
├── artifacts/
│   Compiled smart contract artifacts
│   Used for deployment and integration
│
├── attest_submit.js
│   Script for submitting verification attestations to blockchain
│
├── fetch_all_events.mjs
│   Script for retrieving historical blockchain event logs
│   Used for audit and verification purposes
│
├── package.json
│   Project dependencies and runtime scripts
│
├── .env.example
│   Template for environment variables
│   (API keys, cloud credentials, etc.)
│
└── .gitignore
    Specifies files that should not be committed
    (node_modules, secrets, etc.)
