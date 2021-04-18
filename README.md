CSE 130 asgn2
Adarsh Sekar
adsekar@ucsc.edu
1619894

Note:
This program will not work on unix, as there are a few methods that only work on linux.
To get it to work on UNIX, you must remove the define POSIX_C_SOURCE 200809L line and define GNU_SOURCE line
You may also have to change some of the ways I use getopt, as some things I do are specific to Linux.

This README is for asgn2, the multithreaded httpserver. The file should have a Makefile, httpserver.c, httpfunc.c and httpfunc.h to run. To compile simply call make or make all. To run the program, run ./httpserver with a port number, and an optional -N and -l header.
The -N header must be followed by an positive integer number of threads, and the -l header a name for a log file. 
As of the time this README is written, there are no known errors that will occur when running the program. 
An earlier version of the program when run on the git test script, failed on simultaneous PUT, GET and HEAD, and some other requests, but on the current version has not been run with the git test script.
However, when performing such tests locally on the current version, there were no errors.