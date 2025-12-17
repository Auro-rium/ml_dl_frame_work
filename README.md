# Machine Learning and Deep Learning Workspace

This repository is for testing, experimentation, and learning by getting hands dirty with core machine learning and deep learning workflows. It contains a collection of Jupyter notebooks and scripts covering NumPy, pandas, scikit-learn, PyTorch, computer vision, and more.

## Quick links

- **Deep Learning (PyTorch)**
  - [dl/repl.ipynb](dl/repl.ipynb)
  - [dl/fundamentals_dl0.ipynb](dl/fundamentals_dl0.ipynb)
  - [dl/fundamentals_dl1.ipynb](dl/fundamentals_dl1.ipynb)
  - [dl/classification_dl2.ipynb](dl/classification_dl2.ipynb)
  - [dl/computervision_dl3.ipynb](dl/computervision_dl3.ipynb)
  - [dl/datasets_dl4.ipynb](dl/datasets_dl4.ipynb)
  - [dl/tranferlearning_dl5.ipynb](dl/tranferlearning_dl5.ipynb)

- **Machine Learning Libraries**
  - [library_learning/ml_numpy.ipynb](library_learning/ml_numpy.ipynb)
  - [library_learning/pandas.ipynb](library_learning/pandas.ipynb)
  - [library_learning/scikitlearn0.ipynb](library_learning/scikitlearn0.ipynb)

- **The Annotated Transformer**
  - [annotated-transformer/AnnotatedTransformer.ipynb](annotated-transformer/AnnotatedTransformer.ipynb)
  - [annotated-transformer/the_annotated_transformer.py](annotated-transformer/the_annotated_transformer.py)

- **Modular Scripts**
  - Overview: [dl/going_modular/README.md](dl/going_modular/README.md)
  - Entry point: [dl/going_modular/going_modular/train.py](dl/going_modular/going_modular/train.py)

## Structure

- **`dl/`**: Deep learning notebooks, small datasets, and modular scripts.
  - `going_modular/`: Reusable Python scripts for training.
  - `data/`: Datasets used in notebooks (e.g., `pizza_steak_sushi`, `FashionMNIST`).
  - `models/`: Exported PyTorch checkpoints.
- **`library_learning/`**: Machine learning notebooks focusing on libraries like NumPy, pandas, and scikit-learn.
- **`annotated-transformer/`**: Implementation of "The Annotated Transformer" paper, including notebook and Python script versions.
- **`helper_functions.py`**: General utility functions used by multiple notebooks.

## Quick start

1. Create a Python environment (recommended Python 3.10+).
2. Install core packages used across notebooks:
   ```bash
   pip install numpy pandas matplotlib scikit-learn jupyterlab notebook torch torchvision
   ```
3. Open the desired notebook in VS Code or Jupyter and run cells.

### Notes
- Some notebooks/scripts assume recent PyTorch + torchvision versions.
- For modular training scripts, read [dl/going_modular/README.md](dl/going_modular/README.md) first.

## Running Modular Training

1. Prepare data (see [`going_modular.data_setup.create_dataloaders`](dl/going_modular/going_modular/data_setup.py)).
2. Run the training script:
   ```bash
   python dl/going_modular/going_modular/train.py
   ```

## Contributing
- Make small, focused changes.
- Update relevant notebook outputs if you change code behavior.

## License
This workspace is intended for learning and personal use. No license file is included.
