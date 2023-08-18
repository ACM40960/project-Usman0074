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

1. **Data Collection and Preprocessing:**

   Historical Premier League data is compiled from a variety of sources. Match statistics such as match fixtures, results, goals, shots, corners, cards received, and Bet365 probabilities are retrieved from https://www.football-data.co.uk/. Defensive ratings for teams are derived from WhoScored (https://www.whoscored.com/) and are available in the provided 'Defending_Prem.xlsx' file.


2. **Feature Engineering:**

   Key features are engineered, including team form, shot accuracy, defensive performance, chances created, and booking points. These features offer critical insights into team dynamics.
We also check how these features affect the possibility of a team scoring goals.

<img src="https://github.com/ACM40960/project-Usman0074/blob/main/Images/Correlation of features with home goals.png">
<img src="https://github.com/ACM40960/project-Usman0074/blob/main/Images/Correlation of features with away goals.png">

We also check how the home and away goals scored in the Premier League are distributed, and since it's a count, we model it against the Poisson distribution.

<img src="https://github.com/ACM40960/project-Usman0074/blob/main/Images/Home Goal Distribution.png">
<img src="https://github.com/ACM40960/project-Usman0074/blob/main/Images/Away Goal Distribution.png">



