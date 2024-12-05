This is the readme for the model code for the paper

Artificial evolution of neurons optimized for specific computations.
Klaus M. Stiefel and Terrence J. Sejnowski
Journal of Neurophysiology

This model code was contributed to ModelDB by Klaus Stiefel..

How to run the demonstration files:

1. If you have not already done so, install NEURON. 

Windows, Linux and OS10 versions of this program can be downloaded
free of charge from

http://www.neuron.yale.edu/neuron/install/install.html

2. Run GA.hoc to start a run of the genetic algorithm. During each
generation, the morphologies of the first 16 neurons of the population
and their somatic membrane potentials are plotted. The parameters of
the genetic algorithm (population size, mutation rates …) can be
modified in the first block of GA.hoc. The extent of the synapse-space
can be modified in template.hoc.

3. The simulation will save a text-file “Generation#.txt” after
completion of each generation.  To load the best performing neuron of
a generation, run LOAD_WINNER.hoc, specify the generation and press
the “Load” button.

4. The code runs the optimization for linear summation. If you would
like to change it to spike-order detection, to change GA.hoc in lines
98, 99 and lines 83, 84 so that "ordertest.hoc" is loaded and
executed, and

	 LOAD_WINNER.hoc in lines 31, 32 and 55, 56.

6/8/2007 version update: a short run test was added to auto-launch options

Changelog
---------
2024-11: Updated hoc files to use Random123
