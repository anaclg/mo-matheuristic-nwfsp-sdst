# Multi-objective matheuristic for minimization of total tardiness and energy costs in a steel industry heat treatment line

## About

This repository contains the dataset used in the evaluation of the multi-objective matheuristic proposed in the manuscript entitled "Multi-objective matheuristic for minimization of total tardiness and energy costs in a steel industry heat treatment line" published by Ana C. L. Gomes, Martín G. Ravetti and Eduardo G. Carrano at Computers & Industrial Engineering, Volume 151, January 2021. Below are the manuscript details.

> Ana Cristina Lima Gomes, Martín Gómez Ravetti, Eduardo G. Carrano \
> \
> Multi-objective matheuristic for minimization of total tardiness and energy costs in a steel industry heat treatment line \
> \
> Computers & Industrial Engineering, Volume 151, 2021, 106929, ISSN 0360-8352, https://doi.org/10.1016/j.cie.2020.106929. \
> \
> Abstract: This research focuses on solving a scheduling problem in a heat treatment line of a multinational steel company. A bi-objective model is proposed to minimize the line total energy costs and total tardiness. The solution is carried out through a matheuristic technique that combines metaheuristics and mathematical programming. A Mixed Integer Linear Programming (MILP) model is designed to generate initial solutions to a Multi-objective Variable Neighborhood Search (MOVNS) algorithm. One benefit of this approach is the ability to handle large-scale problems, common in real production scheduling cases, with reasonable computational time and alternative quality planning. The suggested matheuristic is proven to be statistically superior to an only metaheuristic approach, taking as performance metric the final approximated Pareto solutions’ hypervolume. Tests performed with data from the industry showed improvements in the scheduling of the heat treatment line with reductions of energy costs and tardiness up to 13% and 90%, respectively. The methodology can also be extended to other similar scheduling processes. \
> \
> Keywords: Scheduling; No-wait flow shop; Matheuristic; Multi-objective optimization; Energy consumption; Steel industry

The optimization parameters of the test instances and its usage instructions can be found [here](instances/real-case/inputs). The raw ouput data of the computational experiments is also shared [here](instances/real-case/outputs) with the R script (R version 3.6.3) used to generate the manuscript result tables, figures, and statistical analysis. 

You can also access the manuscript [support information file](docs/support_information_file.pdf) in this repository.

## License

The content of this project is licensed under the Creative Commons Attribution Share Alike 4.0 International license.
