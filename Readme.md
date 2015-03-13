#CScript++

CScript++ is a utility for running C++ (and C and just about anything else that uses Make) projects like Python scripts. I got tired of running make every time I made a code change, so I set up this quick Bash script to automate the build & run process.

Usage:

From the build directory:

`cscript (executable name) (executable options)`
Runs make in directory then calls `executable name` with given options
    
To run outside project build directory, use the `-f (build directory)` option. This `make`s the project in the given directory, then copies the executable to the current working directory and runs it.

To build and run the project in the given build directory, use the `-l` option

To make a target other than the default, use the `-m (target)` option.