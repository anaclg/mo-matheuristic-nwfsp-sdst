# Computational Experiments - Instances Outputs

The outputs from the computational experiments described in the manuscript "Multi-objective matheuristic for minimization of total tardiness and energy costs in a steel industry heat treatment line" are present in the folder [data-csv](data-csv).

## Details of the computational experiments

The data is from 30 executions of the proposed matheuristic and 30 executions of the MOGVNS algorithm initialized with a simple heuristic. The experiments were executed in an 8GB RAM Ubuntu 18.04 LTS server.

## How is the output data organized

The raw results from the experiments are shared as CSV data with the filenames as 'instanceX-30exec-15s.csv'. Each row of the file contains the results from one execution of the algorithm. The columns are:

* Instance: instance identification;
* RealSolution: the cost functions of the sequence executed in reality. The  first value is the total tardiness (TT) followed by a space and the total energy cost (TEC);
* Execution: execution number (from 0 to 29);
* Initial Method: the method used to generate the initial solutions for the MOGVNS algorithm. The "MILP" value refers to the proposed matheuristic executions and the "Heuristics" the MOGVNS initialized with common heuristics;
* NumGroupsTEC (only for MILP initial method): number of jobs considered in the minimization of TEC after applying the grouping strategy;
* TimeTEC (only for MILP initial method): runtime of MILP to minimize TEC in seconds;
* GapTEC (only for MILP initial method): the gap of MILP to minimize TEC (if the solver reached the 1h maximum runtime);
* NumGroupsTT (only for MILP initial method): number of jobs considered in the minimization of TT after applying the grouping strategy;
* TimeTT (only for MILP initial method): runtime of MILP to minimize TT in seconds;
* GapTT (only for MILP initial method): the gap of MILP to minimize TT (if the solver reached the 1h maximum runtime);
* TimeTT_TEC (only for MILP initial method): runtime of MILP to minimize TEC after TT in seconds;
* GapTT_TEC (only for MILP initial method): the gap of MILP to minimize TEC after TT (if the solver reached the 1h maximum runtime);
* InitialCostFunctions: cost functions of the initial solutions found by the InitialMethod. The first value is TT followed by a space and TEC;
* Algorithm: this column only identifies the metaheuristic applied, which will always be MOGVNS-FI;
* RunTimeSec: the runtime of the MOGVNS_FI run in seconds;
* NumParetoSolutions: the number of solutions in the final approximated Pareto front (PF);
* CostFunctions: the cost functions of each solution of the final approximated Pareto (used to draw the charts). A pipe "|" separates the values from different solutions, and first, there are the total tardiness and then, separated by a space, the total energy costs. Example for a 3 solutions PF: 'sol1(TT) sol1(TEC) | sol2(TT) sol2(TEC) | sol3(TT) sol3(TEC)';
* Solutions: the final sequences given by each solution of the final approximated Pareto front. A pipe "|" separates them, and they are ordered according to the CostFunctions column.

In this folder, you will also find an R script (R version 3.6.3) that can be executed to generate the tables and statistical analysis from the CSV files.
