# Driven composite systems and interface with QuTiP in scQubits

Systems of interest in quantum computing generally involve mutual coupling between multiple quantum systems.
By driving these individual subsystems, we can perform single- or multi-qubit gates.

In the context of superconducting circuits, a common method of driving a circuit is to capacitively couple a voltage bias to one or multiple nodes of the circuit. 
By a proper choice of drive frequency, amplitude and envelope, logical operations can be achieved.

The popular Python package QuTiP can be used to simulate the time dynamics of quantum systems. 
For the simulation of superconducting circuits, scQubits provides a transparent interface to QuTiP through the `HilbertSpace` class.

These notebooks showcase how scQubits can be easily used to simulate dynamics of driven superconducting circuits through examples from the literature. The notebook
`FluxoniumRestTutorial.ipynb` provides a tutorial for using scQubits to simulate the heavy-fluxonium initialization procedure described in [Universal fast flux control of a coherent, low-frequency qubit](https://journals.aps.org/prx/pdf/10.1103/PhysRevX.11.011010) by Zhang et al. The notebook `FluxoniumCZTutorial.ipynb` contains a tutorial for using scQubits to simulate the procedure for effecting a CZ-gate on a coupled pair of fluxonium qubits described by Nesterov et al. in [Microwave-Activated Controlled-Z Gate for Fixed-Frequency Fluxonium Qubits.](https://arxiv.org/abs/1802.03095)

## Dependencies

* python: 3.7.0
* numpy: 1.21.6
* qutip: 4.7.1
* matplotlib: 3.5.3