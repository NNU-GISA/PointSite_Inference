# PointSite Inference Tool
## Setup

Tested with CUDA 10.0, Ubuntu 18.04, Python 3.6 with [Conda](https://www.anaconda.com/) and PyTorch 1.1.

```
# Install related library, e.g
conda install pytorch torchvision cudatoolkit=10.0 -c pytorch # See https://pytorch.org/get-started/locally/
conda install google-sparsehash -c bioconda
conda install -c anaconda pillow
git clone git@github.com:PointSite/PointSite_Inference.git
cd PointSite_Inference/
bash develop.sh
```
 
