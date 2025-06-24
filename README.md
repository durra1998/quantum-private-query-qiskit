# quantum-private-query-qiskit
Implementing a Quantum Private Query protocol using W-state and Qiskit with noise analysis


This project implements a **Quantum Private Query (QPQ)** protocol based on entangled **W-state** particles, simulated using the [Qiskit](https://qiskit.org/) framework. The protocol allows a user (Alice) to privately query a single bit from a database owned by another party (Bob), **without revealing** which bit she accessed.

The implementation is based on the published paper:  
📄 **"Quantum Private Query Using W-State"**, *International Journal of Theoretical Physics*  
DOI: [10.1007/s10773-020-04653-4](https://doi.org/10.1007/s10773-020-04653-4)

---
## 📂 Dataset

We use the **Breast Cancer Wisconsin Dataset** from the UCI ML repository. The `"diagnosis"` column is converted into a binary list (M = 1, B = 0) to simulate a real-world queryable database.

---

## 🚀 Features

- Full implementation of the W-state-based QPQ protocol
- Simulation of **gate and measurement noise** using Qiskit Aer
- Accuracy analysis over multiple queries
- Heatmap visualization showing noise sensitivity of the protocol

---

## 🧠 Background

In this protocol, Alice, Bob, and Charlie share a **3-qubit W-state**. By performing measurements in randomly chosen bases (Z or X), Alice and Charlie can establish a secret key unknown to Bob, which Alice later uses to decrypt one bit of Bob’s encoded database.

This project simulates this interaction and examines its performance in the **Noisy Intermediate-Scale Quantum (NISQ)** era, where quantum processors are powerful but prone to noise.

> 📚 Reference:
> - Yang, Y.G., et al. (2020). [Quantum Private Query Using W-State](https://doi.org/10.1007/s10773-020-04653-4). *IJTP*

---

> 🔍 Key Insight: Measurement noise is more detrimental to protocol success than gate noise. The protocol remains effective for **low to moderate noise levels**, making it promising for near-term quantum devices.

---

