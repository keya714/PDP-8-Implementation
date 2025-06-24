# 🖥️ PDP‑8 CPU Implementation (Logisim-Based)

This project is a **digital logic-level simulation** of the **PDP‑8 CPU**, implemented using **Logisim**. It replicates the architecture and functioning of the original PDP-8 computer, one of the earliest and most influential minicomputers developed by **Digital Equipment Corporation (DEC)**.

---

## 📚 Overview

The PDP‑8, first released in 1965, was a groundbreaking machine due to its affordability and simplicity. Known as the "Model T of the computer industry," it introduced the world to accessible computing and became the best-selling computer by the early 1970s.

This project reconstructs the PDP-8 CPU architecture using basic logic gates and digital circuits in Logisim, emphasizing educational value and hands-on understanding of how early computers worked internally.

---

## 🧠 Features

- ✅ 12-bit instruction word architecture
- 📦 Program Counter (PC), Accumulator (AC), Link Register (L)
- ⚙️ Modified addressing mode implementation
- 🧮 Group 1 & Group 2 micro-instruction support
- 🖼️ Fully visual logic-level design in Logisim

---

## 🛠️ Methodology

- **Instruction Set Basics**:
  - **Word size**: 12 bits
  - **Registers**:
    - PC (12 bits)
    - AC (12 bits)
    - L (1 bit) – acts as a carry/borrow flag
  - **Instruction Word Format** (original):
    - `op` – 3-bit opcode
    - `i` – indirect addressing bit
    - `z` – page bit
    - `addr` – 7-bit address offset

- **Modified Design in This Project**:
  - Introduced **two indirect bits** to support:
    - `00` – direct
    - `01` – immediate
    - `10` – register direct
    - `11` – indirect addressing

- **Micro-instruction Support**:
  - Group 1: Operations on Accumulator and Link (e.g., CLA, CLL, COM, etc.)
  - Group 2: Conditional skips and flags (e.g., SMA, SZA, OSR)

---
