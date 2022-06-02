# RTSA-lab01-SchedulabilityTest
In this lab session you will learn how to implement the schedulability tests for:

  * Liu and Layland Bound
  * Time Demand Analysis
  * Hyperbolic Bound

All Tasks are periodic, preemptable, fixed priority Tasks with implicit Deadlines.

The task sets are defined int the text files in 'task_sets/'.

## Implementing the Tests

The tests  can be found in 'schedTests/' folder in their corresponding files.
The test() functions are called, if the test was successful it should return True, otherwise False. For the TDA test the code for sorting the task set is already included, so the task set is ordered by highest priority first.

The tasksets are represented by a 2D array, where row i is a Task i and the columns contain period(P_i), Deadline (D_i) and WCET (C_i). This is stated in each file with a large comment and examples are given.


## Runing the Tests

Make sure you have at least python3, argparse, numpy and tabulate installed.
Argpoarse and Numpy can be installed via pip.

Use the SchedTest.py Script

```
usage: SchedTest.py [-h] --i I --n N

A small Scheduling test Framework.

options:
  -h, --help  show this help message and exit
  --i I       Path to the file containing task sets.
  --n N       Number of tasks per set.
```

N is always and defaults to 10, for our input files.

## Setup
I guess everyone has a running python setup on his machine.
If not follow this [guide](https://code.visualstudio.com/docs/python/python-tutorial).

But we recommend VS Code, as debug tasks are provided in this repo.
Also make sure to install the python and pylance extension in VS Code.
