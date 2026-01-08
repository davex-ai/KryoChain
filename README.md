# ❄️ KryoChain
### A Minimal Blockchain Implementation in Java

🚀 **KryoChain** is a lightweight blockchain written in **pure Java**, built to explore the core mechanics behind decentralized ledgers: blocks, transactions, wallets, hashing, and chain validation.

This project is **educational**, **hackable**, and designed to grow.

---

## 🧊 Features

✅ Proof-of-Work mining  
✅ Immutable block structure  
✅ Wallets with public/private keys  
✅ Signed transactions  
✅ Transaction validation  
✅ Blockchain integrity checks  

---

## 🏗️ Core Architecture
```
kryochain/
├── Block.java
├── Transaction.java
├── Wallet.java
├── Blockchain.java
└── Main.java

```

---

## 📦 Class Overview

### 🔗 Block
Represents a single block in the blockchain.

**Responsibilities:**
- Stores transaction data
- Links to the previous block via hash
- Performs mining using Proof-of-Work

**Key Fields:**
- `hash`
- `previousHash`
- `timestamp`
- `nonce`
- `List<Transaction> transactions`

---

### 💸 Transaction
Represents a transfer of value between wallets.

**Responsibilities:**
- Holds sender & recipient addresses
- Stores transaction value
- Digitally signs transactions
- Verifies authenticity

**Key Fields:**
- `sender`
- `recipient`
- `amount`
- `signature`

---

### 👛 Wallet
Represents a blockchain user.

**Responsibilities:**
- Generates public/private key pairs
- Signs transactions
- Tracks balance

**Key Fields:**
- `PrivateKey privateKey`
- `PublicKey publicKey`

---

## 🔐 Cryptography

KryoChain uses:
- **SHA-256 hashing**
- **ECDSA digital signatures**
- **Public-key cryptography**

This ensures:
- Tamper resistance
- Transaction authenticity
- Wallet security

---

## ⚙️ How Mining Works

⛏️ Mining adjusts the block’s `nonce` until the hash meets the difficulty target:

0000xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx


The more leading zeros → the harder it is.

---

## ▶️ Running the Project

```bash
javac *.java
java Main
```

You’ll see:

Blocks being mined

Transactions being created

Chain validation results

🧪 Example Output
⛏️ Mining block...
✅ Block mined: 0000a94f2c...
💸 Transaction signed
🔗 Blockchain valid: true

🧠 Why KryoChain?

This project exists to:

Understand blockchain fundamentals

Learn cryptography in practice

Build systems from first principles

Avoid “black box” frameworks

Made with 💖 by [Dave](https://github.com/davex-ai)
