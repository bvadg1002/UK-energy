# UK Energy Analysis — Technical Interview Notebook

This repository contains a Jupyter notebook, `uk_energy_analysis.ipynb`, that explores historic UK electricity demand and generation with lightweight, interview-focused analysis. 


<img width="1100" height="500" alt="image" src="https://github.com/user-attachments/assets/8bb19ac9-e983-4f6e-b5e0-2ac8dbe7f8bd" />



## Contents
- Exploratory analysis of national demand from 2009 to 2024 with resampling and rolling statistics
- Clean plots with Matplotlib and interactive visuals with Plotly
- Simple error metric calculation for sanity checks on trends
- Clear, readable code that can be discussed during a technical interview


## Notebook outline
- Load libraries and configuration
- Load demand and generation data, parse, clean and join them.
- Resample to investigate energy demand trends at different time scale
- Compute rolling means and baseline forecast for the future 48h window
- Train `GradientBoostRegression` models with different features
- Compare forecasting ML models with the baseline 
- Assess feature importance for the ML models
- Short conclusions and discussion points


## Data
Primary external sources:
Demand data from [Kaggle](https://www.kaggle.com/datasets/albertovidalrod/electricity-consumption-uk-20092022/data) retrived using `kagglehub`
Generation data from [NESO Energy API](https://www.neso.energy/data-portal/historic-generation-mix/historic_gb_generation_mix#) retrieved using `requests`

Once retrieved the datasets are saved to /data as .csv files.


## Getting Started

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/bvadg1002/uk_energy.git
    cd uk_energy
    ```

2. **Install Dependencies:**

Make sure you have Python and Jupyter installed. You can install required packages using:
    ```bash
    pip install -r requirements.txt
    
3. **Launch the Notebook:**
    ```bash
    jupyter notebook notebooks/adaptfy_uk_energy.ipynb
    ```

## Usage

- Follow the instructions and code cells in the notebook to analyze, visualize, and optimize your energy data.
- All code, documentation, and results are contained within the repository. No additional scripts are required.

## License

This project is licensed under the MIT License.

## Contact
Authored by Vadim Bogatyr. Questions and ideas are welcome.

