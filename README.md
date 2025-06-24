# quantum-private-query-qiskit
**Simulating a Quantum Private Query protocol using W-state and Qiskit with noise analysis**


This project implements a Quantum Private Query (QPQ) protocol based on entangled W-state particles, simulated using the [Qiskit](https://qiskit.org/) framework. The protocol allows a user (Alice) to privately query a single bit from a database owned by another party (Bob), without revealing which bit she accessed. Its performance is examined in the **Noisy Intermediate-Scale Quantum (NISQ)** era, where quantum processors are powerful but prone to noise<sup>[1]</sup>. By incorporating realistic noise models (including gate error and measurement noise), we assess the feasibility of implementing a Quantum Private Query (QPQ) protocol on NISQ-era hardware.

The implementation is based on the published paper<sup>[2]</sup>:  
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

## 🔍 Key Insight
Measurement noise is more detrimental to protocol success than gate noise. The protocol remains effective for **low to moderate noise levels**, making it promising for near-term quantum devices.

---

## 📚 References

[1] Preskill, J. (2018). *Quantum Computing in the NISQ era and beyond*. Quantum, 2, 79.  
DOI: [10.22331/q-2018-08-06-79](https://doi.org/10.22331/q-2018-08-06-79)

[2] Yang, Y.G., et al. (2020). *Quantum Private Query Using W-State*. International Journal of Theoretical Physics.  
DOI: [10.1007/s10773-020-04653-4](https://doi.org/10.1007/s10773-020-04653-4)

---



