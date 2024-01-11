# CPU Temps - Alexander Lasson 01059661 
This program will takes the readings from 4 cores 
in a CPU. 

CPU Temperature Monitoring System

Overview

Welcome to the CPU Temperature Monitoring System project! This project was developed as part of a college assignment to create a tool for monitoring and analyzing the temperature of a computer's central processing unit (CPU). The goal was to provide users with real-time information about their CPU temperature, allowing them to make informed decisions about system performance and cooling.

Features

Real-time Temperature Monitoring: The system provides continuous monitoring of the CPU temperature, displaying the data in a user-friendly interface.
Graphical Representation: Temperature data is visualized through graphs, enabling users to observe trends and fluctuations over time.
User Alerts: Customizable temperature thresholds trigger alerts to notify users of potential overheating issues. This feature helps users take preventive measures before critical situations occur.
Data Logging: The system records historical temperature data, allowing users to review past performance and identify patterns.
Cross-Platform Compatibility: The project is designed to be cross-platform, ensuring compatibility with various operating systems.

Each reading was taken in 30 second intervals.

The program takes the reading from the input files of each core and 
finds the line of best fit and outputs the point of best fit for 
each point with least squares.

Program consist of Doxyfile layout

The program will provide the output of interpolation at each point.

# Requirements
> gcc

> GNUmake

> Boost 1.71.0 (https://www.boost.org/users/download/)

# Project Layout
## build
> compiled src code excluding the program executable

## Include
> .h files

## resources
> Resource files, CPU temp readings.

## src
> Source code


# Setup/Compilation & Execution Instructions  
- Untar package.
- modify the makefiles under the project directory and the test directory and 
supply the path to the apporiate BOOST_ROOT 
(currently set at the convention of /usr/local/boost_#LibNumber#)

boost_1_71_0 was used 

You may specify your boost directory when GNUmake 
is ran by issuing the following command:

- make BOOST_ROOT='/your/boost/dir'
- make test 


## To Run:
> ./CPUTemps res/sensors-2018.12.26-no-labels.txt

