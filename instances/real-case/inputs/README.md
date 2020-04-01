# Computational Experiments - Instances Inputs

The input data of the 24 instances used in the computational experiments of manuscript "Multi-objective matheuristic for minimization of total tardiness and energy costs in a steel industry heat treatment line" are present in folder [data-xlsx](data-xlsx).

## How is the input data organized

For each instance, there is an Excel file (format .xlsx) that contains the optimization parameters shown in the table below.

| Parameter | Description |
|-|-|
| p_i | total process time of job i throughout all machines [h] |
| p´_i | process time to enter all pieces of job i in the first machine [h] |
| p´_ik | process time of a piece of job i in machine k [h] |
| s_irk | setup time of job r in machine k, when job i precedes job r [h] |
| d_ir | minimum delay at the start of job r, when job i precedes job r [h] |
| v_i | total volume of gas used during execution of job i throughout all machines [Nm3/h] |
| v_ir | total volume of gas used to setup all machines for job r, when job i precedes job r [Nm3/h] |

In the Excel file, there is one sheet (tab) per parameter. The first row of each sheet has the parameter description.

For 1d arrays, the parameter index is shown in the first column and the value in the second column. For 2d arrays, the indexes are in the first column and second row and the parameter values are displayed as a matrix.

For the setup times, which are a 3d array, the values per machine were separated in individual sheets - machine 2 does not appear, because the setup times for it are all zero.