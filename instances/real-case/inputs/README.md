# Computational Experiments - Instances Inputs

The input data of the 24 instances used in the computational experiments of manuscript "Multi-objective matheuristic for minimization of total tardiness and energy costs in a steel industry heat treatment line" (under submission) are present in folder [data-json](data-json).

## How is the input data organized

For each instance, there is a file that contains the optimization parameters in [JSON](https://www.json.org/json-en.html) format. The parameters are shown in the table below.

| Parameter | Description | JSON variable name |
|-|-|-|
| p_i | total process time of job i throughout all machines [h] | ProcessTimeTotal |
| p´_i | process time to enter all pieces of job i in the first machine [h] | ProcessTimeByJob |
| p´_ik | process time of a piece of job i in machine k [h] | ProcessTimeByJobAndMachine |
| s_irk | setup time of job r in machine k, when job i precedes job r [h] | SetupTime |
| w_ir | waiting time to start job r, when job i precedes job r [h] | WaitingTime |
| v_i | total volume of gas used during execution of job i throughout all machines [Nm3/h] | VolumeGasByJob |
| v_ir | total volume of gas used to setup all machines for job r, when job i precedes job r [Nm3/h] | VolumeGasIdleTime |

Each instance file also contains the parameters grouped by temperature (GroupByTempParameters) and due date (GroupByDateParameters). They are used in the MILP runs to generate the initial solutions.
