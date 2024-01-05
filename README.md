# DistilVPR

(AAAI 2024) DistilVPR: Cross-Modal Knowledge Distillation for Visual Place Recognition

<img src="https://github.com/sijieaaa/DistilVPR/blob/main/teaser.png" width=400>



## Installation

- Platform

  ```
  Ubuntu 20.04
  python 3.8
  CUDA >= 11.8
  PyTorch >= 2.0
  ```

- PyTorch

  ```
  pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
  ```

- MinkowskiEngine  https://github.com/NVIDIA/MinkowskiEngine 

  ```
  conda install openblas-devel -c anaconda
  pip install pip==22.3.1
  pip install -U git+https://github.com/NVIDIA/MinkowskiEngine -v --no-deps --install-option="--blas_include_dirs=${CONDA_PREFIX}/include" --install-option="--blas=openblas"
  ```

- Others

  ```
  pip install scikit-learn
  pip install tqdm
  pip install pytorch-metric-learning==1.1
  pip install tensorboard
  ```



## Dataset

The datasets are uploaded at Google Drive. Please download them and unzip them. You need to change some arguments in `tools/options.py` as the directories:

```
--dataset
--dataset_folder
--image_path
```

The teachers' weights are stored in `teacher_weights/`



## Run

We currently provide examples where the teacher is MinkLoc++ and the student is ResNet18+GeM (MinkLoc++2D):

```

```



## Citation

```
@article{wang2023distilvpr,
  title={DistilVPR: Cross-Modal Knowledge Distillation for Visual Place Recognition},
  author={Wang, Sijie and She, Rui and Kang, Qiyu and Jian, Xingchao and Zhao, Kai and Song, Yang and Tay, Wee Peng},
  journal={arXiv preprint arXiv:2312.10616},
  year={2023}
}
```
