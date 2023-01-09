# Driven composite systems and interface with QuTiP in scQubits

Systems of interests for quantum computing generally involve mutual coupling between multiple quantum systems.
By driving these individual sybsystems, we can perform single- or multi-qubit gates.

In the context of superconducting circuits, a common method of driving a circuit is to capacitively couple a voltage bias to one or multiple nodes of the circuit. 
By a proper choice of drive frequency, amplitude and envelope, logical operations can be achieved.

The popular Python package QuTiP can be used to simulate the time dynamics of quantum systems. 
For the simulation of superconducting circuits, scQubits provides an easy and transparent interface to QuTiP through the `HilbertSpace` class.

This set of notebooks provides a three-part tutorial showcasing how scQubits can be easily used to simulate dynamics of driven superconducting circuits.
The first tutorial, contained in `CircuitDrivingTutorial.ipynb`, lays out the theory and provides a walkthrough of the process for building the simulation. The notebooks
`FluxoniumRestTutorial.ipynb` and `FluxoniumCZTutorial.ipynb` provide sample applications using examples from the literature.

## Dependencies

python - 3.10.8
scqubits - 3.1.0
numpy - 1.22.4
qutip - 4.7.0
matplotlib - 3.5.1
