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

### ✨ Highlighting
- Highlight all instructions referencing a selected variable  
- Highlight all label references  

### 🐞 Debugger
- Step-by-step execution  
- Current-line highlight  
- Live variables (`x`, `z`, `y`) with change highlights  
- Real-time cycle counter  
- Jump + EXIT handling  

### 🕒 Run History
- View all previous runs  
- Open any run state snapshot  
- Re-run with identical inputs & settings  

---

# 🌐 3. Client–Server Platform

## 🖥️ Server (Tomcat)
REST endpoints:

- Upload programs  
- List programs & functions  
- Execute program (architecture + degree)  
- Credit deduction & validation  
- Run history retrieval  
- Connected users overview  

## 💻 Client (JavaFX)
- Login screen  
- Live dashboard (users, programs, functions)  
- XML upload  
- Add credits  
- Select: Program → Architecture → Degree → Run  
- View results (`y`) and cycle count  
- Per-user run history  

---

# 📂 4. XML Test Files

The repository includes several XML test programs for:

- Simple executions  
- Heavy synthetic instruction expansion  
- QUOTE & function composition  
- Invalid programs (for error validation)  
- Large scale performance tests  

Usage:
- GUI → FileChooser  
- Server → Upload Endpoint  
- Console → Path Input  

---

# 🧾 Summary

**S-Emulator** is a fully integrated software system featuring:

- 🔧 Generalized execution engine  
- 📈 Multi-level synthetic expansion  
- 🖥️ JavaFX front-end with debugging tools  
- 🌐 Distributed Client–Server support  
- 👤 User + credit management  
- 🕒 Run history, validation, and program visualization  
- 🧪 Comprehensive XML test file suite  

It is a complete end-to-end platform combining logic, UI, networking, debugging, and program execution for the S-Language.

---
