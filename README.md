# Cloud Solutions for quantum computing for the Maximum cut problem

Maximum cut is an NP-complete problem.  No polynomial-time algorithms for Max-Cut in general graphs are known. Running it on a Quantum computer can theoretically reduce the compute time.


## About the problem

The aim of Max-cut is to maximize the numbers of edges
in a graph that are “cut” by given vertices into two sets. For
a graph, a maximum cut is a cut whose size is at least the
size of any other cut. That is, it is a partition of the graph&#39;s
vertices into two complementary sets S and T, such that the
number of edges between the set S and the set T is as large
as possible. The problem of finding a maximum cut in a
graph is known as the Max-Cut Problem.
The formal definition of this problem is the following:
Consider an n-node undirected graph G = (V, E) where |V| =
n with edge weights wij&gt;0, wij=wji, for (i,j) ∈ E. A cut is
defined as a partition of the original set V into two subsets.
The cost function to be optimized is in this case the sum of
weights of edges connecting points in the two different
subsets, crossing the cut.

Max-Cut is an NP-complete problem, with applications in
clustering, network science, and statistical physics. To grasp
how practical applications are mapped into given Max-Cut
instances, consider a system of many people that can
interact and influence each other. Individuals can be
represented by vertices of a graph, and their interactions are
pairwise connections between vertices of the graph, or
edges. Therefore, for every quantum computer that we
accessed, we created an example of the maximum cut
problem with 4 graph nodes and random weights. This setup
was done using the Python network library for creating and
analyzing weighted undirected graphs. We used matplotlib
to draw the resultant graph and store it in the IDE or display
it in Jupyter Notebook

## Running the algorithm D-Wave Quantum System

Create a free tier account on https://cloud.dwavesys.com/leap/

Open an empty workspace and copy the python file in the LEAP IDE provided by DWave.

Open a Terminal and run the following command

```bash
python max_cut.py
```

The result will be displayed in form of an image and saved in the same directory.

## Running the algorithm on IBM Quantum Experience
Create a new Jupyter Notebook on IBM Q platform

Import required libraries like qiskit

Create an example of the maximum cut problem

Convert the problem to a Ising Formula

Choose the available IBM Quantum system or simulator

Results displayed in the Jupyter Notebook


## Running the algorithm on AWS braket
Create Sagemaker (Jupyter) notebook instance.

Create S3 bucket and link it with notebook instance

Import braket SDK.

copy the code from file `Amazon-Braket-MaximumCut.ipynb`

Choose the hardware device to run on.

Choose number of shots

Submit task to the QPU

When job is completed, AWS cloud watch event is created.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
