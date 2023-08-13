# Anaconda Setup

## Anaconda Installation

* <https://www.anaconda.com/download>
* Make sure Python 3.8-3.11 is installed (Compatibility to PyTorch)

 `python --version`

## GPU Installation

* Install CUDA: <https://anaconda.org/nvidia/cuda>

 `conda install -c "nvidia/label/cuda-11.8.0" cuda`

* Install PyTorch: <https://pytorch.org/get-started/locally>

 `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`

## Packages required in course

* NodeJS   (For fixing server errors)

 `conda install -c conda-forge nodejs`

* scikit-learn

 `conda install -c anaconda scikit-learn`

* datasets

 `conda install -c conda-forge datasets`

* torchtext

 `conda install -c pytorch torchtext`

## Start Lab within Anaconda Prompt

* Jupyer Lab

 `jupyter lab`

* Or Jupyter Notebook

 `jupyter notebook`

## Test GPU (CUDA)

* Check within Anaconda Prompt:

 `nvidia-smi`

* Or within notebook:

 `torch.cuda.is_available()`

## Updating

* Update conda package manage

 `conda update conda`

* Update Anaconda

 `conda update anaconda`

* Jupyter Lab

 `conda update jupyterlab`

## Anaconda troubleshoot

* List revisions

 `conda list --revisions`

* Install Revision REVNUM

 `conda install --revision REVNUM`

 Note: `conda install --rev 0`  will remove your root environment and the conda command!

* Removing

 `conda remove PACKAGE`

* Full Reset

 `conda install anaconda-clean`

 `anaconda-clean --yes`

* Backup / Restore

 `conda env export --name base --file base_environment.yml`

 `conda env create --name new_base --file base_environment.yml`
