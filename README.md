# Incremental PCA for Streaming Multidimensional Data (C++ / Python)

This library is inspired by the method from:

**Takanori Fujiwara, Jia-Kai Chou, Shilpika, Panpan Xu, Liu Ren, Kwan-Liu Ma**  
_"An Incremental Dimensionality Reduction Method for Visualizing Streaming Multidimensional Data"_  
IEEE TVCG, Vol. 26, No. 1, pp. 418–428, 2020.  
[DOI: 10.1109/TVCG.2019.2934433](https://doi.org/10.1109/TVCG.2019.2934433)

## Features

- Fast C++ backend using [Eigen3](https://eigen.tuxfamily.org/)
- Python bindings via [Pybind11](https://github.com/pybind/pybind11)
- Mental map preservation (Procrustes transformation)
- Supports missing feature handling and uncertainty estimation
- Designed for streaming high-dimensional data

## Requirements

- C++11 compiler
- Python 3.x
- Eigen3, Pybind11, NumPy

Tested on macOS, Ubuntu 22.04+, and Windows 10 (MSVC).

## Installation

### macOS

```bash
python3 presetup.py
pip3 install .
Ubuntu / Linux
bash
Copy
Edit
sudo apt update
sudo apt install libeigen3-dev python3-pip python3-dev
python3 presetup.py
pip3 install .
Windows (MSVC required)
Install Microsoft C++ Build Tools

Install Python 3

Open x64 Native Command Prompt for VS and run:

bash
Copy
Edit
python3 presetup.py
pip3 install .
Usage
Python
python
Copy
Edit
from inc_pca import IncPCA
See sample.ipynb or docs/index.html for examples.

C++
Include inc_pca.hpp and inc_pca.cpp in your project.

Resources
Demo & Paper Evaluation Code

Citation
Please cite the following if you use this code:

Fujiwara, T., Chou, J.-K., Shilpika, Xu, P., Ren, L., & Ma, K.-L.
An Incremental Dimensionality Reduction Method for Visualizing Streaming Multidimensional Data
IEEE Transactions on Visualization and Computer Graphics, 26(1), 418–428, 2020.
DOI: 10.1109/TVCG.2019.2934433
