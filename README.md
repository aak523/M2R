This repository contains the code used to calculate **severability** for a large network, to generate some visulations/analysis for the second graph used.

We undertook this analysis for a second-year Maths group research project, on the topic of Random Walks on Graphs, at Imperial College London. Many thanks to our supervisor Prof. Mauricio Barahona, as well as Juni Schindler and Tim Liu for their support.

We found a **Twitter interaction network** for the 117th United States Congress, both House of Representatives and Senate, and thought it might be interesting to analyse. The base data was collected via Twitter’s API, then the empirical transmission probabilities were quantified according to the fraction of times one member retweeted, quote tweeted, replied to, or mentioned another member’s tweet. For more information, check out [the relevant paper](https://pmc.ncbi.nlm.nih.gov/articles/PMC10493874/).

As discussed in our paper, we did initially convert the given directed graph into an undirected graph to apply severability. This process (`sev_gen_undirected.ipynb`) gave us the data in `congress_severability.csv`. Then, our analysis can be found in `sev_analysis_undirected.ipynb`.

We also briefly experimented with the original directed form of the graph (`sev_directed.ipynb`).

### Requirements
- *Used throughout:* NumPy, pandas, NetworkX.

- *For plotting:* seaborn, Matplotlib.

You will also need to install the [severability library](https://github.com/barahona-research-group/severability), as described in their `README`.

### Dataset Source
[Twitter Interaction Network for the US Congress](https://snap.stanford.edu/data/congress-twitter.html)

### Author
Adam Kassam (@[aak523](mailto:adam.kassam23@imperial.ac.uk))