# Introduction

The [original code](https://github.com/marakeby/pnet_prostate_paper.git) use Python 2.7.15. However, it is not compatible with some of the package. Therefore, I use Python 3.6 environment, most of the packages now can be successfully installed. I rewrite codes from Python2 to Python3 without changing the meaning. Follow the step below to set up the environment and run the code.


# Steps

## Create conda environment



```python
conda create -n pnet python=3.6
conda activate pnet
```


## Install packages

All the packages in the original report can be installed except for the plotly-orca, but it will mot matter since it is not used

* dependencies

```python
pip install plotly
pip install enum34==1.1.6
pip install futures
pip install h5py==2.9.0rc1
conda install hdf5
pip install imageio==2.6.1
pip install keras==2.2.4
pip install keras-applications==1.0.8
conda install keras-base==2.2.4
conda install keras-preprocessing=1.1.0
conda install markdown==3.1.1
pip install numpy==1.16.6
pip install pandas==0.23.4
pip install plotly==4.5.4
pip install protobuf==3.11.2
pip install pyyaml==5.1.1
pip install scikit-image==0.14.2
pip install scikit-learn==0.20.1
pip install scipy==1.1.0
pip install subprocess32==3.5.4
pip install tensorboard==1.12.2
pip install tensorflow==1.12.0
conda install yaml==0.1.7
```
* pip

```python
pip install adjusttext==0.7.3
pip install lifelines==0.19.5
pip install matplotlib==2.2.4
pip install networkx==2.2
pip install pyvis==0.1.7.0
pip install requests==2.23.0
pip install rope==0.18.0
pip install seaborn==0.9.1
pip install toml==0.10.2
pip install upsetplot==0.4.0
pip install urllib3==1.25.8
pip install xlrd==0.9.0
```

## Add Project Directory to system path

In Linux:

export PYTHONPATH=~/pnet_prostate_paper:$PYTHONPATH

Windows:

Click environment variable


## Run code

### Analysis

To generate all paper figures, run

```
cd ./analysis
python run_it_all.py
```

### Train

```
cd ./train
python run_me.py
```

# What I rewrite

Some examples

* print: In python 2, print a. In python 3 print(a)

* open file: In python 2, file(). In python 3 open()

