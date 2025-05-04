# Neural Radiance Fields (NeRF) Project

This project explains, implements and explores Neural Radiance Fields (NeRFs), a method for synthesizing novel views of complex 3D scenes from a sparse set of input views.

## Description

This repository contains code based on the original NeRF paper ([Mildenhall et al., 2020](https://arxiv.org/abs/2003.08934)). It includes:

*   A detailed explanation of NeRF concepts in `projet_nerf_notebook.ipynb`.
*   Implementation of the NeRF model, training pipeline, and rendering process.
*   Scripts/notebooks for training NeRF models and generating novel views (e.g., `generate_views_cpu.ipynb`, `test_nerfs.ipynb`).
*   Example results, including generated views and GIFs.

## Setup

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows use `venv\Scripts\activate`
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: Ensure you have compatible versions of PyTorch/TensorFlow depending on the implementation details, potentially with CUDA support if using a GPU).*

## Usage

*   **Understanding NeRFs:** Open and run the `projet_nerf_notebook.ipynb` notebook for a theoretical explanation and code walkthrough.
*   **Generating Views:** Use `generate_views_cpu.ipynb` or similar scripts/notebooks to render novel views from a trained model.
*   **Training:** (Details might need to be added based on specific training scripts if they exist beyond the main notebook).
*   **Testing:** Use `test_nerfs.ipynb` for testing purposes.

## Project Structure

PAS ENCORE BON, A MODIFIER A LA FIN

```
.
├── articles_nerfs.pdf                # Relevant research paper(s)
├── generate_views_cpu.ipynb          # Notebook for generating views (CPU)
├── projet_nerf_notebook.ipynb        # Main notebook explaining NeRFs
├── requirements.txt                  # Python dependencies
├── test_nerfs.ipynb                  # Notebook for testing
├── generated_views_cpu/              # Output directory for generated views (CPU)
├── gifs/                             # Output directory for animated GIFs of novel views
├── nerf_synthetic/                   # Dataset (e.g., synthetic Lego)
├── nerf_synthetic_lego/              # Specific dataset variant
├── results_for_notebook/             # Images and GIFs used within the main notebook
├── test/                             # Test images/data
├── trained_models/                   # Saved model checkpoints
└── README.md                         # This file
```
