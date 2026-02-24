# FraudNet AI  
### Cross-Channel Mule Account Detection using Graph Intelligence

---

## 🏦 Problem Statement

In modern banking systems, fraudsters increasingly use **mule accounts** to rapidly move stolen funds across multiple banking channels such as UPI, wallets, ATM withdrawals, and inter-bank transfers.  
These transactions individually appear legitimate, but collectively form suspicious patterns that are difficult to detect using traditional rule-based systems.

Banks face challenges in:
- Detecting high-speed, multi-hop fund transfers
- Identifying interconnected mule account networks
- Monitoring cross-channel transaction behavior in real time

---

## 💡 Proposed Solution

**FraudNet AI** is an AI-driven system designed to detect potential mule accounts by modeling banking transactions as a **graph network** rather than isolated records.

The system:
- Represents accounts as nodes and transactions as edges
- Analyzes cross-channel transaction flows
- Detects abnormal movement patterns using machine learning
- Assigns risk scores to suspicious accounts

This graph-based approach enables early detection of mule networks that remain hidden in traditional transaction monitoring systems.

---

## 🧠 Technical Approach

### 1. Data Modeling
- Synthetic transaction data is generated for multiple channels:
  - UPI
  - Wallets
  - ATM
  - Bank Transfers
- Each transaction includes:
  - Source account
  - Destination account
  - Amount
  - Channel
  - Timestamp

### 2. Graph Construction
- **Nodes:** Bank accounts  
- **Edges:** Transactions  
- **Edge Attributes:** Amount, channel, time

Graph analytics helps identify:
- Fan-in / fan-out transaction patterns
- Rapid fund movement across accounts
- Circular and layered transaction flows

### 3. AI-Based Anomaly Detection
- Machine learning models such as **Isolation Forest** are used to detect abnormal transaction behavior
- Each account is assigned a **fraud risk score**
- Accounts exceeding risk thresholds are flagged as potential mule accounts

### 4. Visualization & Monitoring
- A Streamlit-based dashboard displays:
  - Transaction networks
  - Flagged mule accounts
  - Risk scores and alerts

---

## 🛠 Tech Stack

- **Programming Language:** Python  
- **Data Processing:** Pandas, NumPy  
- **Machine Learning:** Scikit-learn  
- **Graph Analysis:** NetworkX  
- **Visualization & Dashboard:** Streamlit  

---

## 🎯 Expected Impact

- Early detection of mule account networks
- Reduction in financial losses due to fraud
- Improved cross-channel transaction monitoring
- Enhanced fraud prevention capabilities for banks

---

## 🚀 Future Enhancements

- Integration with real-time banking transaction streams
- Use of Graph Neural Networks (GNNs) for advanced detection
- Explainable AI for fraud decision transparency
- Scalable deployment for enterprise banking systems

---

## 📌 Conclusion

FraudNet AI demonstrates how **graph intelligence combined with machine learning** can significantly improve the detection of mule accounts in complex, multi-channel banking environments.  
The system provides a proactive and scalable approach to modern fraud prevention challenges faced by financial institutions.

---

**Hackathon Project – Indian Bank | VIT Chennai**
