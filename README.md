# genetic_algorithm
A generalised genetic algorithm module for hamiltonian minimization in any system

The main function of the module is GradDescent which takes the following arguments:
1. Init : Initial State of the system (any type supported by Mutator and Printer functions). Eg - Numpy arrays
2. Mutator : A function that takes in system state and generates mutants. (Inputs : System State)
3. Crossover : A crossover function to merge two system states in order to create recombinant offsprings.
4. H : Hamiltonian function. (Inputs : System State)
5. ofile : An output file to write the results of GradDescent. (Note: This output file should already be open for writing)
6. Printer : A Printer function that converts system state to a string that can be written to the output file.


Usage:
```python
import genetic_algorithm

outputfile = open(<outputfilename>,"w+")

**GeneticAlgo(Init,Mutator,Crossover,H,outputfile,Printer)**

outputfile.close()
```
Contact kbhaskar AT iisc DOT ac DOT in


