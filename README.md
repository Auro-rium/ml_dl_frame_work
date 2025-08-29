# Deep Learning Projects Workspace

This repository contains a collection of deep learning projects and notebooks, primarily focused on PyTorch and computer vision tasks.

## Project Structure

```
classification_dl2.ipynb
computervision_dl3.ipynb
fundamentals_dl0.ipynb
fundamentals_dl1.ipynb
helper_functions.py
ml_project1.ipynb
models/
    01_pytorch_fundamentals_model_0.pth
    01_pytorch_workflow_model_1.pth
data/
    FashionMNIST/
        raw/
            t10k-images-idx3-ubyte
            t10k-images-idx3-ubyte.gz
            t10k-labels-idx1-ubyte
            t10k-labels-idx1-ubyte.gz
            train-images-idx3-ubyte
            train-images-idx3-ubyte.gz
            train-labels-idx1-ubyte
            ...
```

## Contents

- **Jupyter Notebooks**  
  - `fundamentals_dl0.ipynb`, `fundamentals_dl1.ipynb`: PyTorch basics, tensor operations, and linear regression.
  - `classification_dl2.ipynb`: Classification tasks using deep learning.
  - `computervision_dl3.ipynb`: Computer vision workflows with FashionMNIST.
  - `ml_project1.ipynb`: Additional machine learning project(s).

- **helper_functions.py**  
  Contains reusable utility functions for plotting, accuracy calculation, data downloading, and more.  
  See [`helper_functions.py`](helper_functions.py).

- **models/**  
  Stores trained PyTorch model weights (`.pth` files).

- **data/**  
  Contains datasets used in the notebooks, such as FashionMNIST.

## Getting Started

1. **Install Requirements**  
   Make sure you have Python 3.8+ and install dependencies:
   ```sh
   pip install torch torchvision matplotlib numpy
   ```

2. **Run Notebooks**  
   Open any `.ipynb` notebook in [Visual Studio Code](https://code.visualstudio.com/) or Jupyter and run the cells.

3. **Data**  
   The FashionMNIST dataset will be downloaded automatically by the notebooks if not present.

## Helper Functions

Common utilities are available in [`helper_functions.py`](helper_functions.py), such as:
- `plot_predictions`
- `accuracy_fn`
- `plot_loss_curves`
- `download_data`
- `plot_decision_boundary`
- `print_train_time`

## License

This project is for educational purposes.

---

*Created as part of deep learning practice and experimentation with PyTorch.*