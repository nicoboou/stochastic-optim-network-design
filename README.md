# stochastic-optim-network-design

## Problem statement

The French telecommunication company Orange is the unique owner and handler of the telecommunication network in the figure below.

The costs on the links are proportional to the distances d(i, j) between the nodes, expressed in units of 10km. Because of anti-trust regulations, Orange must delegate to another two companies (i.e., SFR and Bouygues) two subnetworks, each having at least two nodes (with
Orange handling the third part). Orange therefore needs to design a backbone network to connect the three subnetworks. Transforming an existing link into a backbone link costs c = 25 e/km.

## Problem formulation

1. **_MIP model formulation:_** Formulate a mathematical (integer linear programming) model to minimize the cost of implementing a backbone connecting the three sub-networks.

2. **_Model implementation and solution:_** Implement the ILP model in Python with Pyomo. Solve the model with the given dataset.

## Data

Backbone updating cost: c = 25e/km
Number of subnetworks: K = 3
Minimum cardinality of subnetworks: m = 2
Node set: N = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13}
Link set E and corresponding distance: {(i, j) : d for (i, j) ∈ E}
{(1, 2) : 1.8,
(1, 7) : 1,
(2, 3) : 1.7,
(2, 5) : 7,
(2, 7) : 2,
(2, 12) : 3,
(3, 4) : 2,
(3, 10) : 6.5,
(4, 5) : 1,
(4, 6) : 2,
(5, 8) : 5,
(5, 10) : 1,
(5, 11) : 1.5,
(6, 11) : 2.1,
(7, 12) : 2,
(8, 9) : 2,
(8, 13) : 0.7,
(9, 10) : 1.1,
(10, 11) : 1,
(12, 13) : 2.5,
(1, 13) : 5.4,
(2, 8) : 2.3, }
2
