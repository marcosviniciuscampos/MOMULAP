For each instance in its respective folder there are the following files:

FRONT_<INSTANCE NAME>.TXT => In each line of this file are the values ​​of the objective functions of the respective non-dominated individual. The first three values ​​refer to coverage, weighted distance and access equity. The next three bring the same information as the previous ones, but in a normalized way and treating all objectives as minimization. The individuals described in this file compose the set of non-dominated individuals for the refered instance resulting from all executions of the NSGA-II and SPEA2 algorithms.


The next five files follow the same pattern, differing from one another by the way the set of non-dominated individuals is generated.


FRONT_<INSTANCE_NAME>_EXISTING.TXT 			=> Set of non-dominated individuals considering existing mammography units
FRONT_<INSTANCE_NAME>_NSGA-II.TXT  			=> Set of non-dominated individuals considering the 30 executions of the NSGA-II algorithm
FRONT_<INSTANCE_NAME>_SPEA2.TXT  			=> Set of non-dominated individuals considering the 30 executions of the SPEA2 algorithm
FRONT_<INSTANCE_NAME>_NSGA-II_EXEC_<#EXEC>.TXT 	=> Set of non-dominated individuals for a executuion of the NSGA-II algorithm
FRONT_<INSTANCE_NAME>SPEA2_EXEC_<#EXEC>.TXT 		=> Set of non-dominated individuals for a executuion of the SPEA2 algorithm



The next two files present the results concern to the Hypervolume and Spacing indicators for each execution of each algorithm. In each line, the execution id, the Hypervolume value and the Spacing value are displayed

INDICATORS_<INSTANCE_NAME>_NSGA-II.TXT 	=> Hypervolume and Spacing results using NSGA-II
INDICATORS_<INSTANCE_NAME>_SPEA2.TXT 		=> Hypervolume and Spacing results using SPEA2


The individual is described in the follow file:

S_<INSTANCE_NAME>_<ALGORITHM>_EXEC_<#EXEC>_<#INDIVIDUAL>.TXT => That file describes an individual generated in one of the executions of an algorithm for a given instance. 

Its content consists of:

- Objective Functions Values
- Location, Allocations and Idle Service of each mammography unit
- List of cities covered by each mammography unit
- List of mammography units by city
- Coverage of Demand by city



