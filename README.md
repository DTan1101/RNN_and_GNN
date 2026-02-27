# PM2.5 Prediction and Graph Learning

This project contains experimental notebooks for two main directions:
- PM2.5 time-series forecasting using RNN/PyTorch.
- Graph Neural Network (GraphSAGE) experiments on the Twitch graph dataset.

## Project Structure

```text
PM2.5/
|- data/
|  |- raw/
|  |  |- Beijing-PM2.5.csv
|  |- external/
|     |- twitch/
|- notebooks/
|  |- rnn.ipynb
|  |- rnn_error.ipynb
|  |- gnn.ipynb
|  |- test_torch.ipynb
|- models/
|  |- best_model_pytorch.pth
|  |- best_model_graphsage.pth
|  |- best_model_graphsage_cora.pth
|- artifacts/
|  |- figures/
|- logs/
|- requirements.txt
|- requirments.txt
|- environment.yaml
`- README.md
```

## Environment Requirements

- Python 3.10 or 3.11
- pip or conda

## Quick Setup

### Option 1: pip

```bash
pip install -r requirements.txt
```

### Option 2: conda

```bash
conda env create -f environment.yaml
conda activate pm25-env
```

## How to Run

1. Start Jupyter:

```bash
jupyter lab
```

2. Open notebooks in `notebooks/` based on your goal:
- `rnn.ipynb`: train/forecast PM2.5 with RNN.
- `rnn_error.ipynb`: analyze forecasting errors.
- `gnn.ipynb`: GraphSAGE/GNN experiments on graph data.
- `test_torch.ipynb`: validate the PyTorch environment.

## Data and Outputs

- PM2.5 dataset: `data/raw/Beijing-PM2.5.csv`
- Twitch graph dataset: `data/external/twitch/`
- Trained models: `models/*.pth`
- Output figures: `artifacts/figures/`
- TensorBoard logs: `logs/`

## Notes

- `requirments.txt` is kept for compatibility with the requested filename.
- When running notebooks, open the workspace at the project root (`PM2.5/`) so relative paths resolve correctly.
