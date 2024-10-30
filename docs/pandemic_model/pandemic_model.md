## Pandemic Model Overview

**Analytic**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tpike3/jupyter_bridge/main?labpath=docs%2Fpandemic_model%2Fmesa_sir.ipynb)

### Description 

This is a pandemic modelling approach known as a S(usceptible), I(infected) and R(ecovered) or SIR model. 

Components of the model are:

**Agents:** Each agent in the model represents an individual in the population. Agents have states of susceptible, infected, recovered, or dead. The Agents are point agents, randomly placed into the environment.

**Environment:** The environment is a set of polygons of a few Toronto neighborhoods.   

**Interaction Rules:** Susceptible agents can become infected with a certain probability, if they come into contact with infected agents. Infected agents then recover after a certain period or perish based on a probability.

**Parameters:** 
- Population Size (number of human agents in the model)
- Initial Infection (percent of the population initial infected)
- Exposure Distance (proximity suscpetible agents must be to infected agents to possibly get infected)
- Infection Risk (probability of becoming infected)
- Recovery Rate (time infection lasts)
- Mobility (distance agent moves)


### Key Features

- **Data Output:** Map of select Toronto Neighborhoods
- **"Hamburger" Menu:** &#9776;  In the upper left of the interface provides ways to change the parameters of model and see the impact on changing the dynamics of the previously listed parameters 
- **Full Screen Button:** &#xe5d0; Upper right makes the dashboard full screen

```{toctree}
---
maxdepth: 0
hidden: true
---

```