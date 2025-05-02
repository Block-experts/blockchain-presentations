---
marp: true
theme: default
_class: invert
---

# Introduction to Blockchain  

#### Understanding the Technology and Its Real-World Impact  

**By ET-TAOUSY Zouhair**

---

#  Failed P2P Systems (Before Bitcoin)

| Name             | Year | Description | Reason for Failure |
|------------------|------|-------------|--------------------|
| **e-gold**       | 1996 | Gold-backed digital currency | Shut down (2009): legal issues |
| **Liberty Reserve** | 2006 | Anonymous USD/EUR transfers | Shut down (2013): money laundering |
| **Beenz**        | 1998 | E-commerce loyalty currency | Failed to scale; shut down ~2001 |
| **Flooz**        | 1999 | Gift currency | Shut down (2001): fraud, low use |
| **DigiCash**     | 1989 | Privacy-focused digital cash | Bankrupt (1998): no traction |
| **GoldMoney (P2P)** | 2001 | Gold as digital money | P2P disabled due to regulation |

---

##  Successful Systems (Before Bitcoin)

| Name         | Year | Description | Status |
|--------------|------|-------------|--------|
| **PayPal**   | 1998 | P2P transfers via email/PDA | Still active, global leader |
| **Alipay**   | 2004 | P2P + e-commerce payment | Dominant in China |
| **WebMoney** | 1998 | Russian P2P and digital wallet | Still active |
| **M-Pesa**   | 2007 | Mobile money via SMS | Huge success in Africa |

---

## Lessons Learned

- Most early systems failed due to **centralization** and **regulatory pressure**
- **Success** came to those who:
  - Solved real problems
  - Embraced regulation (or operated in regulatory gaps)
- **Bitcoin (2009)** was the first **truly decentralized** P2P system

---

# Internet Protocol Layers

 The internet: Layers of open protocola

1. **Link Layer** – Ethernet (physical/data link connectivity)  1974
---

# Internet Protocol Layers

 The internet: Layers of open protocola

1. **Link Layer** – Ethernet (physical/data link connectivity)  1974
2. **Network Layer** – TCP/IP (connectivity)  1974

---

# Internet Protocol Layers

 The internet: Layers of open protocola

1. **Link Layer** – Ethernet (physical/data link connectivity)  1974
2. **Network Layer** – TCP/IP (connectivity)  1974
3. **Application Layer** – HTTP 1990
PIZZA Hut: 1994 (fist sell) PizzaNet

---


# Internet Protocol Layers

 The internet: Layers of open protocols

1. **Link Layer** – Ethernet (physical/data link connectivity)  1974
2. **Network Layer** – TCP/IP (connectivity)  1974
3. **Application Layer** – HTTP 1990
PIZZA Hut: 1994 (fist sell) pizza.net
4. **Application Layer** – SSL/TLS 1996

---

# Internet Protocol Layers

 The internet: Layers of open protocols

1. **Link Layer** – Ethernet (physical/data link connectivity)  1974
2. **Network Layer** – TCP/IP (connectivity)  1974
3. **Application Layer** – HTTP 1990
PIZZA Hut: 1994 (fist sell) pizza.net
4. **Application Layer** – SSL/TLS 1996
5.  **Bitcoin?**

---


# Cryptography ?

---


# Cryptography

## Communications in the presence of adversaries

## SSL/TLS

---

# A Brief History of Blockchain

🧾 Before Bitcoin:
-  **1980s**: David Chaum created **eCash** – a cryptographic digital money
-  Early ideas of privacy, decentralization, and digital signatures
-  Used by banks but never achieved global adoption

2008: Satoshi Nakamoto published the Bitcoin whitepaper  
**"Bitcoin: A Peer-to-Peer Electronic Cash System"**

 Why?
- Reaction to the **2008 financial crisis**
- Wanted a system without banks or central control
- Solved the **double-spending problem** with blockchain + proof-of-work

⚙️ Bitcoin = eCash + blockchain innovation

---

![Satoshi's Email](../assets/bitcoin-email.png)

---

#  What is a Blockchain?

### ⏱️ Timestamped Append-Only Log
- Sequential, time-stamped data
- Immutable (append-only)

###  Auditable Database (Cryptography)
-  Hash functions → **tamper resistance**, **integrity**
-  Digital signatures → **consent**
-  Consensus → **agreement**

### 🔗 Consensus Protocol
- Solves **Byzantine Generals Problem**
- Reduces **“cost of trust”**
- Networks:  Permissioned /  Permissionless
![Satoshi's Email](../assets/blockchain-what-is.png)



---

#  What is Blockchain?

- A Timestemped append-only log
- A **decentralized ledger** of transactions  
- **Immutable**: data cannot be changed once recorded  
- Uses **cryptography** for security  
- Peer-to-peer network, **no central authority**  

 Think of it like a secure, transparent Google Sheet shared by everyone.

---

#  Components of a Blockchain

1. **Blocks** – store data and metadata (hash, timestamp)  
2. **Nodes** – participants in the network  
3. **Consensus Mechanisms** – agree on valid transactions (PoW, PoS)  
4. **Smart Contracts** – self-executing code on-chain  

🔐 Cryptography and decentralization ensure trust and security.

---

graph LR
  Block1["+------------+<br>| Block 1    |<br>+------------+<br>| PrevHash: 0000 |<br>| Tx:          |<br>| - Alice → Bob |<br>| - Carol → Dave|<br>+------------+"]
  Block2["+------------+<br>| Block 2    |<br>+------------+<br>| PrevHash: a1b2 |<br>| Tx:          |<br>| - Bob → Charlie|<br>| - Dave → Eve  |<br>+------------+"]
  Block3["+------------+<br>| Block 3    |<br>+------------+<br>| PrevHash: d4e5 |<br>| Tx:          |<br>| - Eve → Alice |<br>| - Tom → Zoe  |<br>+------------+"]

  Block1 -->|Hash| Block2 -->|Hash| Block


---

# Blocks structure
![Blocks](../assets/blocks.png)

---

# 🔁 Blockchain Generations

1️⃣ **1st Gen** – Bitcoin (digital currency)  
2️⃣ **2nd Gen** – Ethereum (smart contracts)  
3️⃣ **3rd Gen** – Solana, Polkadot, etc. (scalability, interoperability)  

🧱 Each generation solves the limitations of the previous one.

---

# 💻 Smart Contracts

- **What are they?** Programs that run on the blockchain  
- Written in **Solidity (EVM)** or **Rust (Solana, Near)**  
- Deployed and executed by transactions  

🔧 Examples:
- ERC20 token contract  
- NFT minting  
- Decentralized voting  
- Escrow system  

---

# 🔍 Real Use Cases from My Work

✅ **Cryptocurrencies** – Decentralized digital money (e.g., Bitcoin, Ethereum).  
✅ **supply Chain** – Transparent, tamper-proof tracking of goods.  
✅ **Identity Management** – Secure digital IDs (e.g., passports, credentials). 
✅ **Healthcare** – Immutable patient records & drug traceability. 


---

# 🧪 Case Study: Bulk Token Sender App

- Built a web app to **send tokens to hundreds of users at once**  
- Used **Solidity** and **Anchor (for Solana)**  
- Solved gas efficiency, transaction batching, and UI challenges  
- 📦 Deployed on: [bulksendtokens.xyz](https://bulksendtokens.xyz/)  

💡 Reduced airdrop costs and errors for multiple clients.

---

# Discussion