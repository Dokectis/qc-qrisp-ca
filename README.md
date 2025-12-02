# qc-qrisp-ca
qc-qrisp-IQM-Resonance


Qrisp (Quantum RISP) is a high-level, open-source programming framework for quantum computing. It is Python-based and designed to make writing quantum algorithms more like writing standard classical code, rather than manually assembling quantum gates.


While standard frameworks like Qiskit or Cirq often function like "Assembly language" (where you manually place gates on specific qubits), Qrisp functions more like a high-level language (C++ or Python), allowing you to work with variables, functions, and data types.

Here is a breakdown of what Qrisp is and why it matters:

###1. The Core Philosophy: "Variables, not Qubits"
In most quantum frameworks, you manage individual qubits (e.g., "Apply an H-gate to Qubit 0"). In Qrisp, you manage Quantum Variables.


Instead of tracking 5 specific qubits to represent a number, you simply create a QuantumFloat or QuantumInt.

Qrisp handles the low-level logic of which qubits form that variable and how gates should be applied to them.

###2. Key Features
Structured Programming: It supports familiar programming structures. You can write loops and arithmetic operations (like a + b) directly on quantum variables.


Automatic Uncomputation: One of the hardest parts of quantum programming is "cleaning up" temporary qubits (entangled garbage) to save memory and prevent errors. Qrisp automates this cleanup process.

Hardware Agnostic: You write the code in Qrisp, and it compiles down to quantum circuits that can run on various backends, including IBM Quantum, IQM, IonQ, and simulators.

Integration: Since it is Python-based, it integrates smoothly with classical libraries. It is also compatible with Qiskit, meaning you can export Qrisp code into Qiskit circuits if needed.

###3. Who Developed It?
Qrisp was originally developed by Fraunhofer FOKUS (a major German research institute) and is now an Eclipse Foundation open-source project (officially called "Eclipse Qrisp")

### 4. Comparison: Qrisp vs. QiskitFeatureQiskit 

Feature,Qiskit / Cirq,Qrisp
Abstraction Level,Low-Level (Assembly-like),High-Level (Software-like)
Primary Building Block,Qubits & Gates,Quantum Variables & Functions
Arithmetic,You must build adder circuits manually.,You simply type a + b.
Qubit Management,Manual allocation.,Automatic allocation & recycling.


Links:

https://qrisp.eu/index.html

https://github.com/eclipse-qrisp/qrisp

