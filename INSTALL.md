# Installation Instructions

This document provides instructions for setting up the quantum machine learning environment on a new computer.

## Prerequisites

- Python 3.11 (recommended)
- pip (Python package installer)
- git (for cloning repositories)

## Quick Setup

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd qt-master-qml
   ```

2. **Create a virtual environment**:
   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment**:
   - On Linux/macOS:
     ```bash
     source .venv/bin/activate
     ```
   - On Windows:
     ```bash
     .venv\Scripts\activate
     ```

4. **Install all required packages**:
   ```bash
   pip install -r requirements.txt
   ```

## Key Packages Included

### Quantum Computing
- **Qiskit 0.40.0** - Main quantum computing framework
- **Qiskit Aer 0.11.2** - High-performance simulators
- **Qiskit IBM Provider 0.19.2** - Access to IBM Quantum systems

### Data Science & Machine Learning
- **NumPy 2.3.4** - Numerical computing
- **Pandas 2.3.3** - Data manipulation
- **Scikit-learn 1.7.2** - Machine learning algorithms
- **Matplotlib 3.10.7** & **Seaborn 0.13.2** - Data visualization
- **SciPy 1.16.3** - Scientific computing

### Development Environment
- **JupyterLab 4.4.10** - Interactive development environment
- **IPython 9.6.0** - Enhanced Python shell

## Verification

After installation, verify your setup by running:
```bash
python -c "import qiskit; print('Qiskit version:', qiskit.__version__)"
python -c "import numpy; print('NumPy version:', numpy.__version__)"
python -c "import pandas; print('Pandas version:', pandas.__version__)"
```

## Usage

Start JupyterLab to begin working:
```bash
jupyter lab
```

## Troubleshooting

If you encounter issues:

1. **Python version compatibility**: Ensure you're using Python 3.11
2. **Virtual environment**: Make sure the virtual environment is activated
3. **Package conflicts**: Try creating a fresh virtual environment
4. **System dependencies**: Some packages may require system-level dependencies (e.g., build tools)

For system-specific issues, consult the individual package documentation.
