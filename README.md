# 📘 S-Emulator  
A Complete Execution, Expansion & Debugging Environment for the S-Language

---

## 🌟 Overview

**S-Emulator** is a full software ecosystem that emulates the execution and expansion of programs written in the **S-Language** — a minimal, mathematically inspired instruction set with Basic Instructions, Synthetic Instructions, QUOTE, and Function Composition.

The system includes:

- ⚙️ **Core Logic Engine**  
- 🖥️ **Modern JavaFX GUI**  
- 🌐 **Client–Server Architecture (Tomcat + JavaFX Client)**  
- 🐞 **Step Debugger**  
- 📂 **XML Test Programs Suite**  
- 👤 **User Accounts & Credit-Based Execution**

It behaves like a complete programming environment: loading programs, expanding by degree, cycle-accurate execution, debugging, program history, remote execution, and more.

---

# ⚙️ 1. Core Logic Engine

### ✔ Instruction System
- Basic Instructions  
- Synthetic Instructions  
- QUOTE support  
- Function composition  
- Clean OOP hierarchy for all instruction types

### ✔ Program Expansion Engine
- Computes base level and overall expansion degree  
- Multi-level expansion: **degree 0 → max level**  
- Generates expanded instruction trees  
- Stores **history chains** for all expanded instructions  

### ✔ Execution Engine
- Variables: `x1..xn`, `z1..zk`, `y`  
- Jump system with Labels + EXIT  
- Cycle-accurate execution  
- Execution context tracking  
- Complete **run history**: inputs, outputs, cycles, degree  

---

# 🖥️ 2. JavaFX Graphical Interface

### 📄 Program Viewer
- Instruction table (line, type, label, text, cost)  
- Expansion controls with live degree indicator  
- Visualization of expanded instructions  

##
