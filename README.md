# BSD-Fusion
The implementation code of “Breaking Synthetic Dependency: Towards Real-world Unaligned Infrared-Visible Image Fusion”.

## Update
- [2025/10] All code will be open after acceptance.
- ....

## Video Presentation
For more video results, check out the [[project page](https://boyang-pro.github.io/Video_example/)]. 
## Environment

We test the code on PyTorch 2.1.1 + CUDA 11.8.

1. Create a new conda environment
```
conda create -n BSD-Fusion python=3.10
conda activate BSD-Fusion
```

2. Install dependencies
```
conda install cudatoolkit==11.8
pip install torch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu118
pip install setuptools==68.2.2
conda install -c "nvidia/label/cuda-11.8.0" cuda-nvcc
conda install nvidia/label/cuda-11.8.0::cuda-cudart-dev  
conda install nvidia/label/cuda-11.8.0::libcusparse-dev  
conda install nvidia/label/cuda-11.8.0::libcublas-dev  
conda install nvidia/label/cuda-11.8.0::libcusolver-dev  
cd kernels/selective_scan && pip install .
pip install -r requirements.txt
```
