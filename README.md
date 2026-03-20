# EmergingTechnologies

![Python](https://img.shields.io/badge/python-3.8+-blue)
![Qiskit](https://img.shields.io/badge/qiskit-latest-purple)
![Qiskit Aer](https://img.shields.io/badge/qiskit--aer-latest-purple)
![Matplotlib](https://img.shields.io/badge/matplotlib-latest-orange)
![Jupyter](https://img.shields.io/badge/jupyter-latest-orange)

> Quantum algorithm implementation using Qiskit, running on a simulated quantum computer.

An implementation of the [Deutsch–Jozsa algorithm](https://quantum.cloud.ibm.com/learning/en/modules/computer-science/deutsch-jozsa), built as part of an exploration into quantum computing.

The notebook covers generating valid Boolean test functions, solving the constant-vs-balanced problem classically, building quantum oracles and running both Deutsch's single-bit algorithm and the full n-bit Deutsch-Jozsa algorithm on a simulated quantum computer.

## Table of Contents

- [File Structure](#file-structure)
- [Problems](#problems)
- [Getting Started](#getting-started)
- [Documentation & Resources](#documentation--resources)

## File Structure

```
EmergingTechnologies/
├── .gitignore          # Files and folders to be ignored by Git
├── problems.ipynb      # Main notebook covering all 5 problems
├── requirements.txt    # Python dependencies
└── README.md           # Documentation of the project
```

## Problems

All problems are implemented in [problems.ipynb](problems.ipynb).

| Problem | Title | Summary |
|---------|-------|---------|
| [1](problems.ipynb#problem-1-generating-random-boolean-functions) | Generating Random Boolean Functions | Implements `random_constant_balanced()`, a function that randomly generates a constant or balanced 4-bit Boolean function for use as test input to the algorithm |
| [2](problems.ipynb#problem-2-classical-testing-for-function-type) | Classical Testing for Function Type | Implements `determine_constant_balanced()`, which classically determines if a function is constant or balanced, requiring up to 9 queries in the worst case |
| [3](problems.ipynb#problem-3-quantum-oracles) | Quantum Oracles | Builds Qiskit quantum oracle circuits for all four single-input Boolean functions using X gates and CNOT gates |
| [4](problems.ipynb#problem-4-deutschs-algorithm-with-qiskit) | Deutsch's Algorithm with Qiskit | Implements Deutsch's algorithm as a 2-qubit circuit that determines constant vs balanced in a single oracle query using phase kickback |
| [5](problems.ipynb#problem-5-scaling-to-the-deutschjozsa-algorithm) | Scaling to the Deutsch–Jozsa Algorithm | Generalises the circuit to 5 qubits (4 input + 1 target qubit) to handle the 4-bit functions from Problem 1, solving the problem in one query regardless of input size |

## Getting Started

### Prerequisites
- [Python](https://docs.python.org/3/) (>3.8)
- [Qiskit](https://quantum.cloud.ibm.com/docs/en/guides)
- [Qiskit Aer](https://github.com/Qiskit/qiskit-aer)
- [Matplotlib](https://matplotlib.org/)
- [Jupyter Notebook](https://docs.jupyter.org/en/latest/)

---
### Step 1 - Clone the repository
```bash
git clone https://github.com/McDonaghMichael/EmergingTechnologies.git
```
---
### Step 2 - Change Directory
```bash
cd EmergingTechnologies
```
---
### Step 3 - Setup and Activate Virtual Environment
```bash
python -m venv venv
```

In order to activate the environment use one of the following commands based on your OS

**Windows**
```powershell
venv\Scripts\activate
```

**Linux/MacOS**
```bash
source venv/bin/activate
```
---
### Step 4 - Install Dependencies

**Via the `requirements.txt`**
```bash
pip install -r requirements.txt
```

**Manual Installation**
```bash
pip install qiskit qiskit-aer matplotlib jupyter
```
---
### Step 5 - Launch Jupyter Notebook

**Local Server**

Jupyter Notebook Web Interface will by default be available on `http://localhost:8888`
```bash
jupyter notebook
```

**Compatible IDEs/Code Editors**

The following IDEs/Code Editors have Jupyter Notebook capabilities directly or via extensions

- [Visual Studio Code](https://code.visualstudio.com/)
    - [Jupyter Extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- [PyCharm](https://www.jetbrains.com/pycharm/) (Built-in functionality)

## Documentation & Resources

### Resources
- [The Deutsch–Jozsa Algorithm](https://quantum.cloud.ibm.com/learning/en/modules/computer-science/deutsch-jozsa)
- [Deutsch's Algorithm](https://quantum.cloud.ibm.com/learning/en/courses/fundamentals-of-quantum-algorithms/quantum-query-algorithms/deutsch-algorithm)

### Tools and Libraries
- [Python](https://docs.python.org/3/) (>3.8)
- [Qiskit Docs](https://quantum.cloud.ibm.com/docs/en/guides)
- [Qiskit Aer](https://github.com/Qiskit/qiskit-aer)
- [Matplotlib](https://matplotlib.org/)
- [Jupyter Notebook](https://docs.jupyter.org/en/latest/)
