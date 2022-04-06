# RG-JEMOA
ROI generator from Java Evolutionary Multi-Objective Algorithms, this version was developed with C.
# Data type
   * Integer
   * Real (double)
# Problems
  *  DTLZ 1-7
# DTLZ test problems in parallel execution to get optimal fronts without preferences (Linux)
To compile and run parallel from command line the ROI generator it is necessary to execute the following line:
```
./run_parallel NSample Seed numberofObjetives
```
where "NSample" is the size of sample, "Seed" is a seed (Integer) and "numberOfObjetives" is the number of objectives to the problems

#DTLZ test problems in sequential execution to get optimal fronts without preferences (Windows)
First, the file ".c" must be compilated for the execution in Windows OS.
To  run from command line the ROI generator it is necessary to execute the following MS-DOS command:
```
main.exe numberOfProblem NSample Problem_instances_path
```
where "numberOfProblem" is the DTLZ problem to solve, "NSample" is the size of sample, "Problem_instances_path" is the path to the problems instance by objetive.

# Examples
There are here examples of how to execute the roi_generator.  
*  Linux.

Sample = 10k, Seed = 3 and NumberofObjetives = 3.
```
./run_parallel 10000 3 3
```

*  Windows.

Problems =  DTLZ 1,2; numberOfObjetives = 3, 5; NSample = 10k and Problem_instances_path = "..\DTLZ_INSTANCES\$numberOfObjetives\"DTLZ"+$numberOfProblem+"_Instance.txt".
```
main.exe 1 10000 ..\DTLZ_INSTANCES\3\DTLZ1_Instance.txt
main.exe 2 10000 ..\DTLZ_INSTANCES\3\DTLZ2_Instance.txt
main.exe 1 10000 ..\DTLZ_INSTANCES\5\DTLZ1_Instance.txt
main.exe 2 10000 ..\DTLZ_INSTANCES\5\DTLZ2_Instance.txt
```

# Publications
* Castellanos A, Cruz-Reyes L, Fernández E, Rivera G, Gomez-Santillan C, Rangel-Valdez N. Hybridisation of Swarm Intelligence Algorithms with Multi-Criteria Ordinal Classification: A Strategy to Address Many-Objective Optimisation. Mathematics. 2022; 10(3):322. <a href="https://doi.org/10.3390/math10030322" target="_blank">doi.org/10.3390/math10030322 </a>
* Castellanos-Alvarez A, Cruz-Reyes L, Fernandez E, Rangel-Valdez N, Gómez-Santillán C, Fraire H, Brambila-Hernández JA. A Method for Integration of Preferences to a Multi-Objective Evolutionary Algorithm Using Ordinal Multi-Criteria Classification Mathematical and Computational Applications. 2021; 26(2):27. <a href="https://doi.org/10.3390/mca26020027" target="_blank">doi.org/10.3390/mca26020027</a>
