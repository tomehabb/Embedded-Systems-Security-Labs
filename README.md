# Embedded-Systems-Security-Labs

Documentation and implementations of labs from the **Embedded Systems Security** course — exploring hardware, firmware, and IoT security concepts through hands-on attacks, defenses, and analysis on real embedded platforms.

---

## 📚 Course Context
This repository contains the complete lab work for the **Embedded Systems Security** module, part of the **International Master's in Embedded Systems Security** at **Grenoble INP - École Supérieure d'Ingénieurs en Systèmes Avancés et Réseaux (ESISAR)**, Valence, France.

---

## 👥 Team Members (Equal Contributors)
| Name                | GitHub Handle |
|---------------------|-------------------
| **Thomas Ibrahim**  | [@tomehabb](https://github.com/tomehabb) |
| **Muhammed Hamza**  | [@hamza1717](https://github.com/hamza1717) |
| **Lukas Da Roza**   | [@lukas-sr](https://github.com/lukas-sr)  | 
---

## 🛠️ Labs Completed

### 1. [Side Channel Attacks](labs/side-channel/)
**Objective**: Recover cryptographic keys using power consumption and electromagnetic emissions.

- **Target**: AES-128 on STM32F4 (ARM Cortex-M4)
- **Techniques**:
  - Simple Power Analysis (SPA)
  - Correlation Power Analysis (CPA)
  - Electromagnetic Analysis (EMA)
- **Tools**: ChipWhisperer-Lite, Python (NumPy, SciPy), Oscilloscope
- **Key Results**: Full key recovery in < 5,000 traces using CPA

> *“Power traces don’t lie — they whisper the secret.”*

---

### 2. [Differential Fault Analysis (DFA)](labs/dfa/)
**Objective**: Inject faults during AES execution to recover the key via differential analysis.

- **Target**: AES-128 software implementation on AVR ATMega328P
- **Fault Injection**:
  - Voltage glitching (Crowbar circuit)
  - Clock glitching (using FPGA)
- **Analysis**: Fault model validation, faulty ciphertext collection, key recovery via DFA equations
- **Tools**: Arduino Uno, Saleae Logic Pro, Custom glitcher board
- **Key Results**: Key recovered with 2–3 faulty ciphertexts

> *“One bit flipped, one key revealed.”*

---

