========================================================================
Grant_Node2vec
========================================================================

node2vec is an algorithmic framework for representational learning on graphs (ref paper see https://dl.acm.org/doi/abs/10.1145/2939672.2939754). 
Given any graph, it can learn continuous feature representations for the nodes, which can then be used for various downstream machine learning tasks.
The node2vec algorithm used here is to measure the similarity of research subjects listed in the research grants. 
The subject co-occurence networks constructed by the the grants data are weighted and undirected.


/////////////////////////////////////////////////////////////////////////////
Parameters:

dimensions:  Dimensionality of the node vectors.
walk_length:  Lenght of random walks.
num_walks:   Number of random walks.
window_size:  Maximum distance between the current and predicted node within a random walk.
iter:      Number of epochs in SGD
workers:    Number of parallel workers. Default is 8.
p:        Return hyperparameter. Default is 1
q:        Inout hyperparameter. Default is 1
weighted:   Boolean specifying (un)weighted. Default is unweighted.
directed:   Graph is (un)directed. Default is undirected.

/////////////////////////////////////////////////////////////////////////////
