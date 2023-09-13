# Hybrid Anomaly Detection based on IP-Flows Network Statistics
Source code for replication of the experiments in the paper "Assessing the Impact of a Supervised Classification Filter for Flow-based Hybrid Network Anomaly Detection".

### Install Dependencies
Create a new conda environment as in original [GEE implementation](https://github.com/munhouiani/GEE), which this method is heavily based on.
```
conda create -n gee python=3.7.7
conda activate gee 
conda install pyspark=3.0.0 click=7.1.2 jupyterlab=2.1.5 seaborn=0.10.1
conda install pytorch=1.5.1 torchvision=0.6.1 cudatoolkit=10.1 -c pytorch
conda install pytorch-lightning=0.8.4 shap=0.35.0 -c conda-forge
pip install petastorm==0.9.2
```
Next, install Jupyter Notebooks to be able to run the provided notebooks.
```
pip install notebook
```
And run the jupyter server:
```
jupyter notebook
```

### Source Code Structure
Just run the notebooks according to their ordinal number in the name.
| # | Description |
| :-: | :-: |
| 01 | Running pretrained pure anomaly detector on test set |
| 02 | Analysis of results from pure anomaly detector |
| 03 | Training classification prefilter on balanced subset of original train set and enrich anomaly detection results on test set |
| 04 | Analysis of results from hybrid anomaly detector |

## Cite [ToDo]
```bibtex
@article{XXXX,
  author = {Dominik Macko and Patrik Goldschmidt and Peter Pi\v{s}tek and Daniela Chud\'{a}},
  title = {Assessing the Impact of a Supervised Classification Filter for Flow-based Hybrid Network Anomaly Detection},
  journal = {XXXX},
  year = {2023}
}
