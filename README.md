# grover-qiskit
Example code written in Qiskit for solving a generic search problem using Grover's algorithm. This was part of an assignment for a "Fundamentals of Quantum Mechanics" course.

* The code assumes a list of `N=16` items among which only `M=2` are solutions; it is however pretty scalable as the diffuser is written in a general way taking "n" qubits as input.
* The oracle is implemented via a classical function `f(x)` and should be modified accordingly if attempting to scale to a different number of items/solutions.
* The implementation requires 4 qubits represent all the 16 items as quantum states, plus 1 additional ancilla qubit needed for the oracle.
* The simulation shows optimal results for 2 Grover iterations, as expected from theory.

## References
* Qiskit textbook, chapter 3.8, "Grover's algorithm", [LINK](https://qiskit.org/textbook/ch-algorithms/grover.html#introduction)
* M. A. Nielsen and I. L. Chang, "Quantum Computation and Quantum Information", chapter 6, "Quantum search algorithms".
