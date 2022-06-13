# QuantME-Quantum4BPMN

This project contains the definitions for _Quantum4BPMN_, which is an extension of BPMN that supports the _Quantum Modeling Extension (QuantME)_.

For this the following new elements were introduced:
* _QuantumComputationTask_: New task type to abstractly model quantum computations
* _QuantumCircuitLoadingTask_: New task type to load quantum circuits into workflows
* _DataPreparationTask_: New task type to prepare the input state for the given input data by adding a set of gates to the beginning of a quantum circuit
* _OracleExpansionTask_: New task type to expand an oracle contained in a quantum circuit
* _QuantumCircuitExecutionTask_: New task type to execute a quantum circuit on a quantum computer
* _ReadoutErrorMitigationTask_: New task type to mitigate the influence of measurement errors for a quantum computation
* _QuantumCircuitObject_: DataObject extension to transfer data about a quantum circuit between the different Quantum4BPMN tasks
* _ResultObject_: DataObject extension to transfer results of a quantum computation
* _QuantumHardwareSelectionSubprocess_: New sub-process to enable automatic quantum hardware selection for all contained tasks during workflow runtime depending on the properties of circuit within the ingoing QuantumCircuitObject (e.g., depth, width)

The XML Schema definition of the Quantum4BPMN extension can be found [here](https://github.com/wederbn/QuantME-BPMN4Quantum/blob/master/Quantum4BPMN-Extensions.xsd).
