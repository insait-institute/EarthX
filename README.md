
<p align="center">
    <img src="asset/earthmind2.png" alt="Image" width="100">
</p>
<div align="center">
<h1 align="center">EarthMind2: Toward Fine-Grained Spatial and Temporal Understanding for Remote Sensing
</h1>
</div>

<p align="center">
    <a href="http://arxiv.org/abs/2408.09110"><img src="https://img.shields.io/badge/Arxiv-2418.09110-b31b1b.svg?logo=arXiv"></a>
    <a href="https://github.com/insait-institute/EarthMind2-website/index.html"><img src="https://img.shields.io/badge/EarthMind2-Project_Page-<color>"></a>
    <a href="https://github.com/insait-institute/EarthMind2/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow"></a>
</p>

<p align="center">
  <a href="#news">News</a> |
  <a href="#abstract">Abstract</a> |
  <a href="#engine">Engine</a> |
  <a href="#dataset">Dataset</a> |
  <a href="#model">Model</a> |
  <a href="#statement">Statement</a>
</p>


## News


### Environment Setup
```
conda create -n earthmind python=3.10 -y
conda activate earthmind
cd ~/projects/EarthMind2
export LD_LIBRARY_PATH=/opt/modules/nvidia-cuda-12.1.0/lib64:$LD_LIBRARY_PATH
export PATH=/opt/modules/nvidia-cuda-12.1.0/bin:$PATH
# conda install pytorch==2.3.1 torchvision==0.18.1 pytorch-cuda=12.1 cuda -c pytorch  -c "nvidia/label/cuda-12.1.0" -c "nvidia/label/cuda-12.1.1"
pip install torch==2.3.1 torchvision==0.18.1 torchaudio==2.3.1 --index-url https://download.pytorch.org/whl/cu121
pip install -r requirements.txt

# method 1: pip install mmcv==2.1.0 -f https://download.openmmlab.com/mmcv/dist/cu121/torch2.3/index.html 
# method 2 local install:  pip install mmcv-2.2.0-cp310-cp310-manylinux1_x86_64.whl
# method 3 openmim install:
pip install -U openmim
mim install mmengine
mim install "mmcv>=2.1.0"
```

## Statement

### Acknowledgement

This project references and uses the following open source models and datasets. Thanks also to `INSAIT` for computing support.

#### Related Open Source Models

[EarthMind](https://github.com/shuyansy/EarthMind)

### Citation

If you are interested in the following work, please cite the following paper.

```
@article{shu2025earthmind,
  title={EarthMind: Towards Multi-Granular and Multi-Sensor Earth Observation with Large Multimodal Models},
  author={Shu, Yan and Ren, Bin and Xiong, Zhitong and Paudel, Danda Pani and Van Gool, Luc and Demir, Begum and Sebe, Nicu and Rota, Paolo},
  journal={arXiv preprint arXiv:2506.01667},
  year={2025}
}
```
