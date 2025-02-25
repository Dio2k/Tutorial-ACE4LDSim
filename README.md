## Introduction 

**Tutorial-ACE4LDSim** is the repository for the tutorial paper "Lattice Dynamics Modeling of Thermal Transport in Solids Using Machine-Learned Atomic Cluster Expansion Potentials: A Tutorial" (J. Appl. Phys. 137, 081101 (2025); doi: [10.1063/5.0251119](https://doi.org/10.1063/5.0251119)). It includes all the data, codes and scripts necessary to **reproduce** the results presented in the tutorial. Some precalculated data of this repository can be accessed at [zenodo](https://zenodo.org/records/14642844), which can be fetched with the codes in `code_available.ipynb`

## Environment

We recommend creating a new environment with Python 3.9.
```
conda create -n tut python=3.9.18
conda activate tut
```

Firstly, we deal with the installation of pacemaker, which is detailed in the origin [document](https://pacemaker.readthedocs.io/en/latest/pacemaker/install/). For convenience, here to quote some pieces:
```
pip install tensorflow==2.8.0 

git clone https://github.com/ICAMS/TensorPotential.git
cd TensorPotential
pip install --upgrade .

git clone https://github.com/ICAMS/python-ace.git
cd python-ace
pip install --upgrade .
```

Secondly, we deal with other packages:
```
pip install hiphive
pip install ase==3.22.1
```

Finally, we install phono3py (see origin [document](https://phonopy.github.io/phono3py/install.html)):
```
conda install -c conda-forge phono3py
```

The `requirements.txt` is also provided.

In addition, to use ACE potential in LAMMPS, please compilate LAMMPS detailed in [here](https://pacemaker.readthedocs.io/en/latest/pacemaker/quickstart/#lammps). To use kaldo package, it has to be installed in a new environment (refer to origin [document](https://nanotheorygroup.github.io/kaldo/docsource/getting_started.html)) due to the conflict with pacemaker.

## Getting started

Start with `code_available.ipynb` right now!

