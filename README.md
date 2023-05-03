
# FL Tutorial (UQ CSSE4011)

Federated learning tutorial given as part of the UQ course on [Advanced Embedded Systems CSSE4011](https://my.uq.edu.au/programs-courses/course.html?course_code=CSSE4011).  
In this tutorial we use [Flower](https://flower.dev/) and [Pytorch](https://pytorch.org/) frameworks.

<img class="aligncenter" style="width:100px" src="imgs/data61-logo.png"/> 

Contact : [Abdelwahed khamis](mailto:abdelwahed.khamis@data61.csiro.au) & [Sara Khalifa](mailto:abdelwahed.khamis@data61.csiro.au) 

---

## Setup
- **Local setup**.  If you wish to run the notebooks locally, type the following in your terminal.
    ```shell
    conda install -c conda-forge flower
    ```
- **Online Notebook**. Just click the "Open in Colab" button below and it will launch it in Google Collab. Ensure that you run the cell with the command below to install requirements
    ```shell
    pip install -q flwr[simulation] torch torchvision matplotlib
    ```
  - **GPU acceleration on Collab** : Runtime > Change runtime type > Hardware acclerator: GPU > Save).  
  - If you see an error related to GPU availability in one of the following sections, consider switching back to CPU-based execution by setting DEVICE = torch.device("cpu"). 




---

## Notebooks
- [Centralized Image Classification](./centralized.ipynb) [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abdelwahed/fl_tutorial/blob/master/centralized.ipynb)
  - Image classification example on CIFAR dataset using Pytorch. 
- [Federated Learning Image Classification ](./FL_1.ipynb) [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abdelwahed/fl_tutorial/blob/master/FL_1.ipynb)
  - Image classification on multiple FL clients using Flower.
