# Hierarchical risk parity using security selection based on peripheral assets of correlation-based minimum spanning trees
## Overview
This repository contains the official code used for the paper 'Hierarchical Risk Parity Using Security Selection Based on Peripheral Assets of Correlation-Based Minimum Spanning Trees' and relevant guidelines for replication.

## Project Structure
```
FRL_GMSC_HRP/
├── requirements.txt                                   # Python dependencies
├── src/                                               # Source code notebooks for portfolio construction and analysis
│   ├── weight_computation_full_correlation.ipynb      # Compute HRP portfolio weights using full correlation
│   ├── weight_computation_gmsc.ipynb                  # Compute HRP portfolio weights using GMSC (global motion subtracted correlation)
│   ├── backtesting_full_correlation_portfolios.ipynb  # Backtest portfolios constructed with full correlation HRP
│   ├── backtesting_gmsc_portfolios.ipynb              # Backtest portfolios constructed with GMSC HRP
│   ├── subperiod_analysis.ipynb                       # Analyze performance across different market subperiods
│   └── visualization.ipynb                            # Generate figures and plots for analysis and results
```
## Installation & Requirements
We recommend using conda environment for installation. For instance:
```
conda create -n hrp_env python=3.8
conda activate hrp_env
pip install -r requirements.txt
```
## Usage
1. Run weight_computation_full_correlation.ipynb and weight_computation_gmsc.ipynb
2. Run backtesting_full_correlation_portfolios.ipynb and backtesting_gmsc_portfolios.ipynb
3. run subperiod_analysis.ipynb and visualization.ipynb

Data will be made available on request.

## Citation 
If you find this work useful for your research, please cite:

```
@article{cho2023hierarchical,
  title={Hierarchical risk parity using security selection based on peripheral assets of correlation-based minimum spanning trees},
  author={Cho, Younghwan and Song, Jae Wook},
  journal={Finance Research Letters},
  volume={53},
  pages={103608},
  year={2023},
  publisher={Elsevier}
}
```

