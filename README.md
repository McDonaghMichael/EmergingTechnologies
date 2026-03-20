# EmergingTechnologies


An implementation of the [Deutsch–Jozsa algorithm](https://quantum.cloud.ibm.com/learning/en/modules/computer-science/deutsch-jozsa), built as part of an exploration into quantum computing.

The notebook covers generating valid Boolean test functions, solving the constant-vs-balanced problem classically, building quantum oracles and running both Deutsch's single-bit algorithm and the full n-bit Deutsch-Jozsa algorithm on a simulated quantum computer.

## File Structure

```
EmergingTechnologies/
├── .gitignore          # Files and folders to be ignored by Git
├── problems.ipynb      # Main notebook covering all 5 problems
├── requirements.txt    # Python dependencies
└── README.md           # Documentation of the project
```

## Getting Started

### Prerequisites
- [Python](https://docs.python.org/3/) (>3.8) 
- [NumPy](https://numpy.org/doc/stable/)
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
### Step 3 - Setup and Activate Virtual Enviorment
```bash
python -m venv venv
```

In order to activate the enviorment use one of the following commands based on your OS

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
pip install numpy qiskit qiskit-aer jupyter
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
- [The Deutsch-Jozsa algorithm](https://quantum.cloud.ibm.com/learning/en/modules/computer-science/deutsch-jozsa)


### Tools and Libraries
- [Python](https://docs.python.org/3/) (>3.8) 
- [NumPy](https://numpy.org/doc/stable/)
- [Qiskit Docs](https://quantum.cloud.ibm.com/docs/en/guides)
- [Jupyter Notebook](https://docs.jupyter.org/en/latest/)