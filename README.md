<p align="center">
  <img width="300" src="https://thumbs.dreamstime.com/z/premier-league-20792019.jpg?w=576" alt="logo">
</p>

# Monte Carlo Simulation of the Premier League based on Modelling Goals Scored

## Introduction
This is a data-driven project that uses statistical analysis, machine learning techniques, and Monte-Carlo simulation to forecast Premier League match outcomes. We have then compared the season results along with the estimated probabilities of each fixture's possible results with the Bet365 probabilities. This README provides a comprehensive explanation of the project's objectives, methods, data sources, model specifics, and usage instructions.

## Project Overview

The **Premier League** is widely regarded as one of the most famous football leagues in the world, famed for its fierce competition and spectacular matches. The primary goal of this project is to develop a predictive model that uses multiple team qualities to forecast the rate parameter. This metric is used to statistically reflect both the home and away teams' goals in a given match. Furthermore, the model seeks to simulate these encounters to take into consideration the intrinsic unpredictability and uncertainty that define football matches.

## Libraries Used

The following Python libraries were used in this project:

```python
import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
import statistics as stat
import seaborn as sns
import statsmodels.api as sm
import statsmodels.formula.api as smf
from scipy.stats import poisson
```

## Methodology

Our predictive model employs a multi-step approach:
