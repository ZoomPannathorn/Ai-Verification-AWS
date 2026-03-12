# 🔍 AI Content Verification & Blockchain Audit Platform

An AI-powered platform for **content authenticity analysis** with **cloud-based audit logging** and **blockchain verification**.

The system verifies the credibility of digital content such as:

- News Articles  
- Online Publications  
- User Generated Content  
- Social Media Posts  

AI evaluates **content reliability**, while results are stored in **cloud infrastructure and blockchain** to ensure **transparency, traceability, and tamper-proof verification**.

---

# 🌟 Key Features

## 🤖 AI Authenticity Scoring

The platform uses **Gemini 2.5 Flash by Google** to analyze content and generate:

- Confidence Score  
- AI Analysis Result  
- Structured JSON Output  

This enables automated **credibility evaluation of digital content**.

---

## 🧹 Data Cleansing Pipeline

The backend **Node.js API** performs preprocessing before AI analysis:

- Input Validation  
- Data Normalization  
- Structured JSON Transformation  

This ensures **consistent and clean input** for AI processing.

---

## ☁️ Immutable Cloud Logging

All analysis results are stored in **Amazon S3 on AWS** to create a secure **audit trail**.

**Benefits include:**

- Historical verification  
- Protection against data tampering  
- Transparent auditing  

---

## ⛓️ Blockchain Verification Registry

A **Solidity smart contract** registers verification records on blockchain.

**Capabilities:**

- Verification record registration  
- Attestation storage  
- Content hash verification  

This ensures that verification records are **immutable, transparent, and publicly auditable**.

---

## ⚙️ Operational Excellence

The system runs in a **production-ready environment** using:

- Amazon EC2 (Amazon Linux)  
- Node.js Runtime  
- PM2 Process Manager  

This allows the service to operate **24/7 with high reliability and scalability**.

---

# 🧠 System Architecture

```text
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
```

---

# 📂 Project Structure

```text
ai-verificationAWS/
│
├── AIVerificationRegistryV2.sol
│   Smart Contract (Solidity)
│   Records verification audit trails on blockchain
│
├── server.js
│   Backend API (Node.js / Express)
│   Handles AI analysis and system integration
│
├── abi.json
│   Smart contract interface (ABI)
│
├── dashboard/
│   React.js frontend dashboard
│
│   ├── src/
│   │   Main UI source code
│   │
│   └── public/
│       Static assets
│
├── artifacts/
│   Compiled smart contract artifacts
│
├── attest_submit.js
│   Script for submitting blockchain attestations
│
├── fetch_all_events.mjs
│   Script for retrieving historical blockchain events
│
├── package.json
│   Project dependencies and scripts
│
├── .env.example
│   Environment variable template
│
└── .gitignore
    Files excluded from Git tracking
```

---

# 🚀 Use Cases

This platform can be applied to:

- Fake News Detection  
- AI-assisted Fact Checking  
- Content Authenticity Verification  
- Digital Evidence Auditing  
- Media Trust Verification  

---

# 📜 License

This project is intended for **research, educational, and prototype purposes**.
