# NP-SAM

## Introduction

In this project we propose an easily implementable workflow for a fast, accurate and seamless experience of segmentation of nanoparticles.

The project's experience could be significantly enhanced with the presence of a CUDA-compatible device; alternatively, Google Colab can be utilized if such a device is not accessible. For a quick access to the program and a CUDA-GPU try our Google Colab notebook. <br>
[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TorbenVilladsen/np-sam/blob/main/NPSAM_GoogleColab.ipynb)

## installation

Clone the repo and create a conda environment. Just copy the code and paste in the terminal for OS X or in Anaconda Prompt for Windows:

(Alternativly, to circumvent Git, download the files manually from the repo and place in same directory)

```
git clone https://oauth2:glpat-sqaQGhx_qFWdG3nB7Tx9@gitlab.au.dk/disorder/np-sam.git
cd np-sam

conda create -n NPSAM python=3.10
conda activate NPSAM

pip install -r requirements.txt
curl -O https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth

conda install -c conda-forge jupyterlab
python -m ipykernel install --user --name NPSAM --display-name NPSAM
```
Similar to Segment Anything, our code requires `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions [here](https://pytorch.org/get-started/locally/) to install both PyTorch and TorchVision dependencies, make sure to stay in the cd and environment. 

### Get started
In the working directory and NPSAM environment execute `jupyter lab` in the terminal. This will launch jupyterlab. 

## Citation
```
@article{NPSAM,
   author = {Larsen, Rasmus and Villadsen, Torben L. and Mathiesen, Jette K. and Jensen, Kirsten M. Ø and Bøjesen, Espen D.},
   title = {NP-SAM: Implementing the Segment Anything Model for Easy Nanoparticle Segmentation in Electron Microscopy Images},
   journal = {ChemRxiv},
   DOI = {10.26434/chemrxiv-2023-k73qz-v2},
   year = {2023},
   type = {Journal Article}
}
```

## Acknowledgment
This repo benefits from Meta's [Segment Anything](https://github.com/facebookresearch/segment-anything). Thanks for their great work.


