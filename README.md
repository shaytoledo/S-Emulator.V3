S-Emulator – Full Project Description

S-Emulator is a complete software system that emulates the execution, expansion, and management of programs written in the S language — an abstract mathematical language built on a very small set of basic instructions, extended with synthetic instructions, functions, and program composition.

The system provides a fully integrated environment that includes:
a logical execution engine, a rich JavaFX graphical interface, a debugging system, and a full Client–Server architecture with user accounts and credit-based execution.

The final product behaves like a real programming environment:
program loading, expansion by degree, execution, step-by-step debugging, function composition, QUOTE operations, architectures, cycle counting, run history, and multi-user cloud usage.

Core Components of the System
1. Logical Engine (Core)

The logical engine is the “CPU” of the system. It is responsible for:

Parsing S-programs from XML files according to a strict schema.

Representing both Basic and Synthetic instructions.

Computing expansion degrees, including:

Base degree for each instruction

Multi-level program expansion (0 → maxLevel)

Maintaining a history chain for every expanded instruction

Full variable model:

x1..xn – input variables

z1..zk – work variables

y – output variable

Full label and jump system, including EXIT.

Complete support for QUOTE and Function Composition.

Accurate calculation of cycle cost for each execution.

Storing complete run history: inputs, outputs, cycles, degree used.

All logic is implemented with clean object-oriented design:
instruction hierarchy, execution context, expansion manager, variable mapping, label remapping, and error-safe XML loading.

2. Full JavaFX Interface

The graphical interface gives the user a powerful interactive environment.

Program View

Table showing every instruction: row number, type (Basic/Synthetic), label, instruction text, cycle cost.

Display of current expansion degree and the maximum degree.

One-click program expansion with full visualization of generated instructions.

Highlighting

Highlighting all instructions that access a selected variable.

Highlighting all instructions that reference a selected label.

Debugger

A fully functional debugging environment:

Step-by-step execution with active line highlight

Live update of variables (x, z, y) after each step

Highlighting variables that changed

Real-time cycle counter

Jump handling and EXIT behavior

Run History System

Complete list of all previous runs

Open any previous run and view all variable states

Re-run programs with the exact same inputs/architecture/degree

XML Loading

Built-in file chooser

Detailed validation errors: missing EXIT, duplicated labels, missing functions, invalid parameters, etc.

3. Full Client–Server Architecture (Tomcat + JavaFX Client)
Server (Tomcat)

The server exposes the logical engine through REST endpoints:

Upload program

Get all programs

Get all functions

User dashboard

Execute program (architecture + degree)

Execution cost and credit deduction

Access run history

Each user has:

User identity

Credit balance

Uploaded programs

Execution history

Client (JavaFX)

Login screen

Live dashboard:

Connected users and statistics

All programs in the system (instruction count, max degree, average cost)

All functions across the system

Upload XML programs to the server

Load credits

Choose program → architecture → degree → run

Results include: output y, cycles, and saved entry in run history

4. XML Test Files

The system includes ready-made test XMLs designed to verify every feature of the engine.

Types of test programs:

Simple programs – validating basic execution

Programs with many synthetic instructions – verifying expansion logic

Programs using QUOTE and function composition

Invalid programs – validating error handling

Long programs – stress and performance tests

Usage

In the GUI: via file chooser

On the server: via upload endpoint

In console tools: by entering the full path

Summary – A Fully Integrated Software Product

S-Emulator is a complete and mature system that includes:

A generalized logical execution and expansion engine

A professional GUI with advanced debugging

Full Client–Server architecture

User and credit management

Full support for the S language and its semantics

Multi-level expansion engine

Program execution, history, highlighting, and error validation

A rich set of XML test files designed for verification

This is a full software ecosystem:
architecture, logic, data model, GUI, server, networking, and deployment — all integrated into one coherent system.
