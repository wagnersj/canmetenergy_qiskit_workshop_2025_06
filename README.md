# NRCan CanmetENERGY - Quantum Workshop - IBM/Qiskit

2025-06-03

## Installing Qiskit

It is recommended that you use Python enviroments for installing Qiskit. You can facilitate this in one of two ways:

- Use the Python Virtual Environments package (```venv```)
- Use Anaconda or Miniconda Python, and the ```conda``` command

NOTE: Mac computers with M-series CPUs may find difficulty when installing Python packages needed for Qiskit. Notably, this includes the ```scipy``` package, which may invoke the installation commands to compile this module from source code. This is a long process and requires that C/C++ development tools are installed on your system. It is recommended that Mac M-series users use the Anaconda/Miniconda route for setting up their Python/Qiskit programming environment, and use the ```conda``` command to install ```scipy``` prior to installing Qiskit packages.

You may prefer using an online Jupyter notebook programming environment (e.g. Google Colab, IBM Watson Studio) instead of installing locally on your computer. If so, you can install the needed Qiskit packages within a notebook cell by running the `pip` commands below.

### Install with Virtual Environments (```venv```)

Check that Python is installed on your system by running the ```python --version``` command. If it is not installed, then download the latest version of Python from: https://www.python.org/downloads/ . If Python is already installed, verify that the version is v3.9 or higher.

Create a Python virtual environment:
```
python3 -m venv /path/to/virtual/environment
```

Activate this new environment:
```
source /path/to/virtual/environment/bin/activate
```

Now, skip to the Install Qiskit packages section for further instructions.

### Install Anaconda Python or Miniconda.

Install Anaconda from here: https://www.anaconda.com/download, OR
install Miniconda from here: https://docs.anaconda.com/miniconda/miniconda-other-installer-links/

Create a conda environment and activate:
```
conda create -n qiskit python=3
conda activate qiskit
```

NOTE: For Mac M-series computers, install the ```scipy``` packages as follows:
```
conda install scipy
```

Now, go to the next section Install Qiskit packages section for further instructions.

### Install Qiskit packages:
```
pip install qiskit qiskit-ibm-runtime
```

Install additional Qiskit packages:
```
pip install qiskit-aer 
```

Install Jupyter and other tools:
```
pip install jupyter matplotlib pylatexenc
```

NOTE: If you are installing within a online Jupyter notebook environment instead of locally on your computer, preface each `pip` command above with an exclaimation point. For example:

```
!pip install qiskit
```

## Links

- Installing Qiskit: https://docs.quantum.ibm.com/guides/install-qiskit
- IBM Quantum Learning: https://learning.quantum.ibm.com/
- Qiskit Addon for SQD: https://qiskit.github.io/qiskit-addon-sqd/