# Probabilistic Logic Circuits

A research and experimental project on **probabilistic logic circuits**, where entropy and measurement principles determine computational outcomes.  
The goal is to develop both a theoretical and practical framework for building logic gates that operate on probabilistic models, potentially enabling faster computation inspired by quantum systems.

---

## Description
**"A probabilistic logic circuit model leveraging entropy and measurement to determine outcomes, offering a novel approach for faster, uncertainty-driven computation in classical and quantum-inspired systems."**

---

## Components
- Theoretical model of probabilistic logic gates  
- Simplified mathematical equations for entropy and measurement  
- Solved examples and applications  
- Potential implementation on classical systems or quantum simulators  

---

## How to Use
1. Review the theoretical model and equations provided.  
2. Apply the probabilistic gate definitions to design logic circuits.  
3. Simulate results using either a classical program (Python/Matlab) or a quantum simulator (Qiskit, Cirq).  
4. Compare multiple measurement outcomes to observe entropy-driven selection of solutions.  

**Example Equation (text only):**  
For a probabilistic AND gate:
Probabilistic Logic Circuits (Summary)

Abstract:
A simplified model for simulating logic circuits using raw probabilities for each gate. Inputs and outputs are represented as probabilities of being 1. Can run on classical or quantum-inspired systems.


---

Probabilistic Logic Gates

AND: P(Y=1) = P(A=1) * P(B=1)

OR: P(Y=1) = P(A=1) + P(B=1) - P(A=1)*P(B=1)

XOR: P(Y=1) = P(A=1)*(1-P(B=1)) + (1-P(A=1))*P(B=1)

NOT: P(Y=1) = 1 - P(A=1)

NAND: P(Y=1) = 1 - P(A=1)*P(B=1)

NOR: P(Y=1) = 1 - (P(A=1) + P(B=1) - P(A=1)*P(B=1))



---

Algorithm (Steps)

1. Initialize input probabilities.


2. Compute gate outputs using above rules.


3. Store outputs for next gates.


4. Extract final probabilities.


5. Optionally, measure outputs as 0 or 1.




---

Example: Probabilistic Full Adder

Inputs: A=0.6, B=0.7, Cin=0.5

Gates:

Temp = XOR(A, B)

Sum = XOR(Temp, Cin)

T1 = AND(A, B)

T2 = AND(Temp, Cin)

Carry = OR(T1, T2)


Outputs (Probabilities): Temp=0.46, Sum=0.73, T1=0.42, T2=0.23, Carry=0.55


---

Advantages

Simple, general model without AI.

Runs on classical or quantum-inspired systems.

Scalable for many inputs and gates.

Suitable for academic publishing.

