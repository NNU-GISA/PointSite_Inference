# PointSite Inference Tool
## Setup

Tested with CUDA 10.0, Ubuntu 18.04, Python 3.6 with [Conda](https://www.anaconda.com/) and PyTorch 1.1.

```
# Install related library, e.g
conda install pytorch torchvision cudatoolkit=10.0 -c pytorch # See https://pytorch.org/get-started/locally/
conda install google-sparsehash -c bioconda
conda install -c anaconda pillow
git clone https://github.com/PointSite/PointSite_Inference.git
cd PointSite_Inference/
bash develop.sh
```
## Inference
 ```
python inference.py 
--gpu: GPU index, if you have not GPU, just ignore it
--output: output root (required)
--data: data root, only support .xyz file (required)
--select_list: TXT file for selected protein name, default None
--num_vote: voting number in inference (default 25, larger number can archieve more stable and high performance)
```
## Visualization
You will get .obj file in output folder, please use MeshLab to visualize.

## Reference
[facebookresearch/SparseConvNet](https://github.com/facebookresearch/SparseConvNet/tree/master/)
