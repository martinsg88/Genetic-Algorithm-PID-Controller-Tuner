Genetic Algorithm PID Controller Tuner
-------------------------------------

Authors
-------

- Stephen Bryant [sbryant31@knights.ucf.edu]
- Daniel Juarez
- Christian Braun


Overview
--------

Uses a genetic algorithm to tune gain values for an abstracted one-dimensional PID controller. Please refer to the screencap for a quick explanation and example of the program's functionality. This program was created as a final project for introduction to robotics at University Of Central Florida

How To Use
----------

- If you wish to create a new map file, edit the control variable NEW_MAP = 1
- For subsequent runs of the program, if you wish to use an existing map, set NEW_MAP = 0
- The map will be located in the same directory as the project, named map.csv
- In a terminal, type python genetic_pid.py
- This will run the simulation.
- Results will be output to the "results" directory.
- Set the control variable RUNS_PER_SCREENSHOT to toggle how many runs you show the champion chromosome's run.
- Results consist of the following:
	- one PNG value every RUNS_PER_SCREENSHOT runs
	- fitness_values_over_time.png, which plots the maximum and average fitness over time
	- champion_gain_values_over_time.png, which plots the evolution of the champion gain values over time

Possible Future Improvements
----------------------------

- Reduce premature convergence on local minima.
- Add parallel populations who independently evolve and then merge
- Improve Line Generation algorithm to make it change smoothly in one direction or the other.


Resources
---------

- The code is self documented
- An introduction to genetic algorithms can be found here: http://www.obitko.com/tutorials/genetic-algorithms/


Requirements
------------

I tried to use as few libraries as possible. I ended up using:
- Matplotlib
- Python 2.7
- "List Tools" module via http://code.activestate.com/recipes/278258/ was included in the project.
