# Neural Radiance Fields (NeRF) Project

This project explains, implements and explores Neural Radiance Fields (NeRFs), a method for synthesizing novel views of complex 3D scenes from a sparse set of input views.

## Description

This repository contains code based on the original NeRF paper ([Mildenhall et al., 2020](https://arxiv.org/abs/2003.08934)). It includes:

*   A detailed explanation of NeRF concepts in `projet_nerf_notebook.ipynb`.
*   Implementation of the NeRF model, training pipeline, and rendering process.
*   Example results, including generated views and GIFs.

The python code essentially consists in modifications of https://github.com/yenchenlin/nerf-pytorch/tree/master, https://github.com/bmild/nerf and chatgpt given code. I don't claim owning the python code present in the repository.
## Setup

I strongly advise to use the onyxia sspcloud plateform (free for INSEE, ENSAE, Polytechnique and other institutions)

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Download the Dataset:**
    Note that should not need to download the dataset since everything is already in the github repository. You should ignore this step, it is just in case.

    The original download link for the synthetic dataset (like the Lego bulldozer) is often broken. You need to download it manually:
    1. Go to the NeRF project page: [https://www.matthewtancik.com/nerf](https://www.matthewtancik.com/nerf)
    2. Find the 'Data' section and click the link for 'NeRF Synthetic Data'. This will likely lead to a Google Drive folder.
    3. Download the `nerf_synthetic.zip` file.
    4. Extract the zip file.
    5. Place the extracted `lego` folder inside a `nerf_synthetic_lego` directory within your project. The final path should look like: `./nerf_synthetic_lego/lego/`


5. **How to run the notebook**
    You can click on run all. However, if you change parameters of the model to conduct experiments, you will need to change the path to the model you just trained in 14th python cell otherwise it will crash.



## Project Structure


```
.


├── projet_nerf_notebook.ipynb        # Main notebook explaining NeRFs
├── requirements.txt                  # Python dependencies
├── gifs/                             # Output directory for animated GIFs of novel views
├── nerf_synthetic_lego/              # Specific dataset variant
├── results_for_notebook/             # Images and GIFs used within the main notebook
├── trained_models/                   # Saved model checkpoints
└── README.md                         # This file
```
