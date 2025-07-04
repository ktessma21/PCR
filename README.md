# Incremental PCA for Streaming Multidimensional Data (C++ / Python)

This library is inspired by the method introduced in:

**Takanori Fujiwara, Jia-Kai Chou, Shilpika, Panpan Xu, Liu Ren, and Kwan-Liu Ma**  
*An Incremental Dimensionality Reduction Method for Visualizing Streaming Multidimensional Data*  
IEEE Transactions on Visualization and Computer Graphics, Vol. 26, No. 1, pp. 418–428, 2020.  
[DOI: 10.1109/TVCG.2019.2934433](https://doi.org/10.1109/TVCG.2019.2934433)

---

## Overview

An efficient C++ and Python implementation of **Incremental PCA** for real-time visualization of high-dimensional streaming data. Includes support for missing features, mental map preservation, and uncertainty estimation.

---

## Features

- C++11 implementation with [Eigen3](https://eigen.tuxfamily.org/)
- Python bindings using [Pybind11](https://github.com/pybind/pybind11)
- Procrustes transformation for mental map preservation
- Position estimation with missing/incomplete data
- Uncertainty quantification for new data points
- Designed for real-time streaming data

---

## Requirements

- C++11 compiler
- Python 3.x
- Eigen3
- Pybind11
- NumPy

Tested on:
- macOS (Sequoia)
- Ubuntu 22.04 LTS
- Windows 10 (MSVC)

---

## Installation

### macOS

```bash
python3 presetup.py
pip3 install .
```

> This installs missing dependencies like Homebrew, pkg-config, Python3, Eigen, and Pybind11.

---

### Linux (Ubuntu)

```bash
sudo apt update
sudo apt install libeigen3-dev python3-pip python3-dev
python3 presetup.py
pip3 install .
```

---

### Windows (MSVC Required)

1. Install [Microsoft Build Tools for C++](https://visualstudio.microsoft.com/downloads/?q=build+tools)
2. Install [Python 3.x](https://www.python.org/downloads/windows/)
3. Open *x64 Native Command Prompt for VS* and run:

```bash
python3 presetup.py
pip3 install .
```

---

## Usage

### Python

```python
from inc_pca import IncPCA
```

See:

- `sample.ipynb` for usage examples
- `docs/index.html` for documentation

---

### C++

```cpp
#include "inc_pca.hpp"
#include "inc_pca.cpp"
```


