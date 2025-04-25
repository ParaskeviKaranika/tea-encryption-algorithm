# Implementation of the TEA Encryption Algorithm in ANSI C

This repository contains an implementation of the **Tiny Encryption Algorithm (TEA)** in ANSI C, along with utilities for correctness verification, performance measurement, and cryptanalysis using linear and differential techniques.

## 🔧 Project Description

### Part 1: Implementation and Correctness Testing

- The **TEA algorithm** is implemented in ANSI C with clear and detailed comments.
- Input/output vector files are generated to validate the implementation:
  - `create_m_c.txt`: Pairs of (M, C) for all M when K = 0.
  - `create_k_c.txt`: Pairs of (K, C) for all K when M = 0.
- Subkeys derived from the key `K = 0x0000a1e9` are calculated for each round:
  - k1 = `________`
  - k2 = `________`
  - k3 = `________`
  - k4 = `________`

### Part 2: Encryption/Decryption Performance

- **1 GiB** of random data (2^26 messages) is generated.
- Encryption/decryption speed is measured:
  - ⏱ Encryption time: `________` sec
  - ⏱ Decryption time: `________` sec
- Results and terminal outputs are included in the `screenshots/` folder.

### Part 3: Cryptanalysis of TEA

- A **linear approximation table** (LAT) is constructed for the substitution box.
- A **difference distribution table** (DDT) is generated for differential analysis.
- The **top 10 linear and differential characteristics** for 3 rounds of TEA are identified and analyzed.
- All related data and explanations are stored in the `analysis/` folder.

## 📂 Project Structure

