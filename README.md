# 🔐 Quantum Key Distribution (QKD) Simulator using BB84 Protocol

## 📌 Overview

This project simulates the **BB84 quantum key distribution protocol**, one of the most foundational and practical quantum cryptographic methods. It demonstrates how **quantum principles** enable two parties—**Alice and Bob**—to securely establish a shared secret key, and how the presence of an eavesdropper (**Eve**) can be detected via increased error rates.

Built using **Python** and **Qiskit**, this simulator serves as a hands-on example of quantum cryptography in action.

---

## 🎯 Project Goals

- Simulate the BB84 QKD protocol
- Demonstrate secure key exchange
- Show how quantum mechanics detects eavesdropping
- Compare error rates with and without interception
- Provide a clean visualization of the process

---

## 🧠 Key Concepts

- **Qubit encoding** in two bases: Rectilinear (+) and Diagonal (×)
- **Random basis selection** by Alice and Bob
- **Quantum measurement & collapse** behavior
- **Eavesdropper detection** by observing error rate
- **Key reconciliation** based on matching bases

---

## 🛠️ Tools & Technologies

| Tool       | Purpose                                  |
|------------|------------------------------------------|
| Python     | Programming language                     |
| Qiskit     | Quantum circuit simulation               |
| Matplotlib | Graphs for error rate comparison         |
| IBM Q Experience | Optional cloud quantum execution  |

---

## 🚀 How It Works

1. Alice generates random bits and bases.
2. She encodes qubits using the chosen bases.
3. Bob selects his own random bases to measure incoming qubits.
4. Alice and Bob share bases over a public channel.
5. They discard mismatched bits and form a raw key.
6. If Eve tries to intercept, the error rate increases.
7. An error rate threshold can help detect eavesdropping.


```

You can change parameters like the number of qubits and whether Eve is present in the `simulate_bb84()` function.

---

## ✅ Sample Keys

```text
Alice Key:  [0, 1, 0, 1, 1]
Bob Key:    [0, 1, 0, 1, 1]
Error Rate: 0.0 %
```

With Eve present:
```text
Error Rate: 24.5 %
```

---

## 📈 Future Improvements

- Add privacy amplification and error correction stages
- Integrate IBM Quantum hardware backend
- Build a web GUI using Flask or Streamlit

---

## 📜 References

- [IBM Qiskit Documentation](https://qiskit.org/documentation/)
- [BB84 Protocol - Wikipedia](https://en.wikipedia.org/wiki/BB84)
- Nielsen & Chuang: Quantum Computation and Quantum Information

