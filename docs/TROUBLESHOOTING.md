# Troubleshooting

## Package import errors

Restart the Colab runtime after installing or changing Qiskit packages, then run cells from the beginning. Avoid mixing an old runtime state with newly installed packages.

## IBM account not found

If Qiskit reports that it cannot find an account for `ibm_quantum_platform`, initialize the service in the new notebook/runtime and save or provide the token using the current IBM Quantum channel instructions. A saved account in one environment is not automatically available in another.

## No backend or long queue

Backend availability and queue length change. Refresh the service, choose an operational backend that satisfies the circuit's qubit requirement, or use the simulator fallback while waiting.

## Transpiled circuit has many qubits

The ISA circuit can display the entire physical register of the selected backend even when the logical circuit uses only a few qubits. Compare circuit depth, operation counts, and the layout mapping rather than assuming that all displayed qubits are active.

## Results differ from the notebook

Sampling variation and hardware noise make exact counts non-deterministic. Compare dominant outcomes and success/error rates. Use the same number of shots when making a quantitative comparison.

## Token safety

If a token was accidentally saved in a notebook or committed, revoke it immediately in IBM Quantum, create a new one, and remove the secret from Git history before sharing the repository.
