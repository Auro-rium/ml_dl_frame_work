# Machine Learning and Deep Learning Workspace

A collection of Jupyter notebooks and small scripts for learning and experimenting with core machine learning and deep learning workflows (NumPy, pandas, scikit-learn, PyTorch, computer vision and small training pipelines). Keep notebooks runnable in VS Code / Jupyter and reusable scripts under `dl/going_modular`.

## Quick links

- Notebooks
  - [dl/repl.ipynb](dl/repl.ipynb)
  - [dl/fundamentals_dl0.ipynb](dl/fundamentals_dl0.ipynb)
  - [dl/fundamentals_dl1.ipynb](dl/fundamentals_dl1.ipynb)
  - [dl/classification_dl2.ipynb](dl/classification_dl2.ipynb)
  - [dl/computervision_dl3.ipynb](dl/computervision_dl3.ipynb)
  - [dl/datasets_dl4.ipynb](dl/datasets_dl4.ipynb)
  - [dl/tranferlearning_dl5.ipynb](dl/tranferlearning_dl5.ipynb)
  - [ml/ml_numpy.ipynb](ml/ml_numpy.ipynb)
  - [ml/pandas.ipynb](ml/pandas.ipynb)
  - [ml/scikitlearn0.ipynb](ml/scikitlearn0.ipynb)

- Script-mode (going modular)
  - Overview: [dl/going_modular/README.md](dl/going_modular/README.md)  
  - Module scripts: [dl/going_modular/going_modular/README.md](dl/going_modular/going_modular/README.md)  
  - Key script files:
    - [dl/going_modular/going_modular/data_setup.py](dl/going_modular/going_modular/data_setup.py) — data helpers and dataloaders
    - [dl/going_modular/going_modular/engine.py](dl/going_modular/going_modular/engine.py) — training / evaluation loops
    - [dl/going_modular/going_modular/train.py](dl/going_modular/going_modular/train.py) — example entry-point to run training

- Utility helpers
  - Root-level helpers: [helper_functions.py](helper_functions.py) — contains helpers like [`helper_functions.download_data`](helper_functions.py), [`helper_functions.set_seeds`](helper_functions.py), [`helper_functions.plot_loss_curves`](helper_functions.py)
  - DL folder copy: [dl/helper_functions.py](dl/helper_functions.py)

- Data and models
  - Data folders: [dl/data/](dl/data/), [ml/data/](ml/data/)
  - Saved models: [dl/models/](dl/models/) and [models/](models/)

## Structure (high level)

- dl/ — deep learning notebooks, small datasets, modular scripts
  - dl/going_modular/going_modular/ — reusable Python scripts for training (see above)
  - dl/data/ — datasets used in notebooks (e.g. `pizza_steak_sushi`, `FashionMNIST`)
  - dl/models/ — exported PyTorch checkpoints
- ml/ — machine learning notebooks (NumPy, pandas, scikit-learn) and sample data
- helper_functions.py — general utility functions used by multiple notebooks
- README.md — this file

## Quick start

1. Create a Python environment (recommended Python 3.8+).
2. Install core packages used across notebooks:
   pip install numpy pandas matplotlib scikit-learn jupyterlab notebook torch torchvision
3. Open the desired notebook in VS Code or Jupyter and run cells.

Notes:
- Some notebooks/scripts assume PyTorch + torchvision recent versions (see top of `dl/repl.ipynb`) and will attempt to install or validate version requirements at runtime.
- For the modular training scripts, read [dl/going_modular/README.md](dl/going_modular/README.md) and the module README [dl/going_modular/going_modular/README.md](dl/going_modular/going_modular/README.md) first.

## How to run the modular training example

1. Prepare data (see): [`going_modular.data_setup.create_dataloaders`](dl/going_modular/going_modular/data_setup.py)
2. Use the training engine: [`going_modular.engine.train`](dl/going_modular/going_modular/engine.py) or run the example entrypoint [dl/going_modular/going_modular/train.py](dl/going_modular/going_modular/train.py).

Example (from repository root):
python dl/going_modular/going_modular/train.py

Read the module READMEs first for expected CLI args / environment.

## Data

- Datasets used by notebooks are under:
  - [dl/data/FashionMNIST/](dl/data/FashionMNIST/)
  - [dl/data/pizza_steak_sushi/](dl/data/pizza_steak_sushi/)
  - [ml/data/](ml/data/)

Notebooks often include code to download or prepare data automatically; see [`helper_functions.download_data`](helper_functions.py) and [dl/going_modular/going_modular/data_setup.py](dl/going_modular/going_modular/data_setup.py).

## Notes

- Keep notebooks reproducible by setting seeds via [`helper_functions.set_seeds`](helper_functions.py).
- If you modify or reuse the modular scripts, prefer the files under `dl/going_modular/going_modular/` (designed to be imported and reused).

## Contributing

- Make small, focused changes.
- Update relevant notebook outputs if you change code behavior.

## License

- This workspace is intended for learning and personal use. No license file is included.
