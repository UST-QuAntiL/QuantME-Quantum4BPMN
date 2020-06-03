# QuantME-BPMN4Quantum

This project contains the definitions for _BPMN4Quantum_, which is an extension of BPMN that supports the _Quantum Modeling Extension (QuantME)_.

For this the following new elements were introduced:
* _QuantumComputationTask_: New task type to abstractly model quantum computations
* _QuantumCircuitCreationTask_: New task type to create quantum circuits
* _DataPreparationTask_: New task type to prepare the input state for the given input data by adding a set of gates to the beginning of a quantum circuit
* _OracleExpansionTask_: New task type to expand an oracle contained in a quantum circuit
* _QuantumCircuitExecutionTask_: New task type to execute a quantum circuit on a quantum computer
* _ReadoutErrorMitigationTask_: New task type to mitigate the influence of measurment errors for a quantum computation
* _QuantumDataObject_: DataObject extension to transfer data about a quantum computation between the different BPMN4Quantum tasks

The XML Schema definition of the BPMN4Quantum extension can be found [here](https://github.com/wederbn/QuantME-BPMN4Quantum/blob/master/BPMN4Quantum-Extensions.xsd).
