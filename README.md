

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)![Python](https://img.shields.io/badge/python-3.6.9-blue.svg) 
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)



## Graph Neural Networks
Lots of learning tasks require dealing with graph data which contains rich relation information among elements.
Modeling physics systems, learning molecular fingerprints, predicting protein interface, and classifying diseases
demand a model to learn from graph inputs. In other domains such as learning from non-structural data like texts
and images, reasoning on extracted structures (like the dependency trees of sentences and the scene graphs of
images) is an important research topic which also needs graph reasoning models. Graph neural networks (GNNs)
are neural models that capture the dependence of graphs via message passing between the nodes of graphs. In
recent years, variants of GNNs such as graph convolutional network (GCN), graph attention network (GAT), graph
recurrent network (GRN) have demonstrated ground-breaking performances on many deep learning tasks, [more reading here](https://arxiv.org/ftp/arxiv/papers/1812/1812.08434.pdf)

## Repository Information
In this repository, I will upload GNN examples along with explanation in the notebooks.
I will use [PyG](https://pytorch-geometric.readthedocs.io/en/latest/) for this because it makes super easy to implement GNN models. Moreover, it has it's own
graph datasets which one can use to learn and customize to their problem domain.

## Installation
PyG installation
```bash
conda install pyg -c pyg
```
Installation via Pip Wheels

1. Ensure that at least PyTorch 1.10.0 is installed:


 ```bash
python -c "import torch; print(torch.__version__)"
 ```
2. Find the CUDA version PyTorch was installed with:
 ```bash
 python -c "import torch; print(torch.version.cuda)"
 ```
3. Install the relevant packages:
```bash
pip install torch-scatter -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
pip install torch-sparse -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
pip install torch-geometric
 ```
 where ${CUDA} and ${TORCH} should be replaced by the specific CUDA version (cpu, cu102, cu113, cu115) and PyTorch version (1.10.0, 1.11.0), respectively. For example, for PyTorch 1.11.* and CUDA 11.3, type:
 ```bash
pip install torch-scatter -f https://data.pyg.org/whl/torch-1.11.0+cu113.html
pip install torch-sparse -f https://data.pyg.org/whl/torch-1.11.0+cu113.html
pip install torch-geometric
  ```
For PyTorch 1.10.* and CUDA 10.2, type:
```bash
pip install torch-scatter -f https://data.pyg.org/whl/torch-1.10.0+cu102.html
pip install torch-sparse -f https://data.pyg.org/whl/torch-1.10.0+cu102.html
pip install torch-geometric
 ```
if you still have any issues, please check the [official installation page](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html) for FAQs and more info.



