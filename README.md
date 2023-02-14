# QuantME-Quantum4BPMN

This project contains the definitions for _Quantum4BPMN_, which is an extension of BPMN that supports the _Quantum Modeling Extension (QuantME)_.

For this the following new elements were introduced:
* _QuantumComputationTask_: New task type to abstractly model quantum computations
* _QuantumCircuitLoadingTask_: New task type to load quantum circuits into workflows
* _DataPreparationTask_: New task type to prepare the input state for the given input data by adding a set of gates to the beginning of a quantum circuit
* _OracleExpansionTask_: New task type to expand an oracle contained in a quantum circuit
* _QuantumCircuitExecutionTask_: New task type to execute a quantum circuit on a quantum computer
* _ReadoutErrorMitigationTask_: New task type to mitigate the influence of measurement errors for a quantum computation
* _WarmStartingTask_: New task type to enable warm-starting a quantum execution by classically pre-computing parameters or solution approximations
* _ResultEvaluationTask_: New task type to evaluate the quality of quantum circuit execution results
* _ParameterOptimizationTask_: New task type to optimize a set of given parameters, e.g., quantum circuit parameters
* _VariationalQuantumAlgorithmTask_: New task type to define a variational quantum algorithm including all of its components on a high level

* _QuantumCircuitObject_: DataObject extension to transfer data about a quantum circuit between the different Quantum4BPMN tasks
* _ResultObject_: DataObject extension to transfer results of a quantum computation
* _ResultEvaluationObject_: DataObject extension to transfer all data related to an execution result evaluation
* _InitialStateObject_: DataObject extension to transfer quantum circuit parameters
* _ParameterizationObject_: DataObject extension to transfer results of a quantum computation
* _QuantumHardwareSelectionSubprocess_: New sub-process type to enable automatic quantum hardware selection for all contained tasks during workflow runtime depending on the properties of the circuit within the ingoing QuantumCircuitObject (e.g., depth, width)
* _CircuitCuttingSubprocess_: New sub-process type supporting circuit cutting and result combination of a given circuit for all contained CircuitExecution tasks

The XML Schema definition of the Quantum4BPMN extension can be found [here](https://github.com/wederbn/QuantME-BPMN4Quantum/blob/master/Quantum4BPMN-Extensions.xsd).
