# Hierarchical Risk Parity using Security Selection based on Peripheral Assets of Correlation-based Minimum Spanning Trees
## Overview
This repository contains the official code used for the paper 'Hierarchical Risk Parity Using Security Selection Based on Peripheral Assets of Correlation-Based Minimum Spanning Trees' and relevant guidelines for replication.

The financial market has an inherent network structure induced by industrial inter-similarities and the intertwined flows of real-world goods and services.
Financial networks have been extensively studied, and correlation-based minimum spanning trees (MSTs) have been a popular analytical tool for understanding them. In this context, the importance of peripheral nodes in a financial network for constructing a robust portfolio has been recognized.

The risk parity strategy aims to build an asset portfolio that is robust to market fluctuations and variations by pursuing equal risk contributions from each asset in the portfolio.
Hierarchical Risk Parity (HRP) effectively incorporates the hierarchical nature of the market by applying an agglomerative hierarchical clustering method to financial time series within the risk parity framework. 

There is a natural connection between the notion of hierarchy in financial markets and the perspective of viewing financial markets as networks, e.g., MST is a special case of hierarchical clustering with the single linkage criterion, and this motivates us to propose portfolios that leverage both standpoints.

Our study proposes hierarchical risk parity portfolios using a new correlation matrix and a security selection method. Specifically, the proposed portfolio comprises selected assets from the peripheral node pool in a correlation-based MST. We used both the full cross-correlation (FC) and global motion subtracted correlation (GMSC). Both correlation matrices maintain—or even improve—portfolio performance compared to benchmarks, but they exhibit different behaviors depending on the number of selected assets and market conditions.

## Project Structure
```
hrp-security-selection-mst/
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
Run the notebooks in the following order:

1. Run weight_computation_full_correlation.ipynb and weight_computation_gmsc.ipynb.
2. Run backtesting_full_correlation_portfolios.ipynb and backtesting_gmsc_portfolios.ipynb.
3. Run subperiod_analysis.ipynb and visualization.ipynb.

Note: Data will be made available upon request. Please contact yc71@illinois.edu for your request.

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

