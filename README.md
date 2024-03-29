# CppNd-Traffic-Simulation-L1

## Summary
  <img src="data/traffic-simulation-L1.gif"/>
  This is project Stage1.
  Udacity CPP Nano degree concurrency project L1, which simulate traffic via concurrency.
  
  **project structure**
  ![project structure](data/traffic-simulation-L1-structure.jpg)

## Dependencies for Buiding 

* cmake >= 2.8
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* OpenCV >= 4.1
  * The OpenCV 4.1.0 source code can be found [here](https://github.com/opencv/opencv/tree/4.1.0)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)
Windows: recommend using MinGW
  make `build` director in top location of project file, then do `make.. && make`, after build 
completed using command `./traffic_simulation` to run.

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./traffic_simulation`.

## Project Tasks

- **Task L1.1** : In the base class `TrafficObject`, set up a thread barrier in its destructor that ensures
that all the thread objects in the member vector` _threads` are joined.

- **Task L1.2** : In the `Vehicle` class, start a thread with the member function `drive` and the
object `this` as the launch parameters. Also, add the created thread into the `_thread` vector of
the parent class.

- **Task L1.3** : Vary the number of simulated vehicles in `main` and use the top function on the terminal
or the task manager of your system to observe the number of threads used by the simulation.
