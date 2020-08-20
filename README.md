## The Problem

How can we model and understand dockless scooter ridership in the UT Austin ecosystem?
Demand is clearly dependent on student presence on campus, but is there more to the story?
We aim to model ridership patterns and trends, understand causal relationships between the broader picture (i.e: car/pedestrian traffic, class meeting periods), efficiently simulate rides for analysis, and forecast future demand.

The City of Austin's [*Shared Micromobility Vehicle* Trips dataset](https://data.austintexas.gov/Transportation-and-Mobility/Shared-Micromobility-Vehicle-Trips/7d8e-dm7r) has ~9.1 million rides. However, we are interested in rides between campus and nearby student housing regions, yielding ~2.5 million rides (~0.86 million to campus, ~1.6 million from campus).

## Code
* [`src/data.py`](src/data.py): data loading and cleaning
* [`src/model.py`](src/model.py): Bayesian network, learning conditional distributions, and sampling (see [`DocklessScooterBayes.ipynb`](DocklessScooterBayes.ipynb))
* [`src/simulator.py`](src/simulator.py): simulates rides and plots regions of high traffic

Built upon my [previous work](https://nimit.io/docklesstraffic.pdf).
