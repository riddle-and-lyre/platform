# JUNIPER Platform

This package contains a release of a software framework for developing and executing JUNIPER applications.
The package includes:

- A Platform - a run-time environment for executing JUNIPER applications (../JUNIPER.Platform/)
- A test JUNIPER application (../JUNIPER.Application.MapReduce/) that counts words in the given input text file (../JUNIPER.Application.MapReduce/input), following the famous MapReduce example of Hadoop 
- A test JUNIPER application (../JUNIPER.Application.MapReduce_OfflineMPI/) that does not require an MPI library (OpenMPI) to be installed

## Prerequisites
- A Java RTE (e.g. https://www.java.com/en/download/)
- Open MPI (can be obtained from https://github.com/open-mpi/). Note that the platform can run without Open MPI in a test configuration
- Apache Maven build tool

## Building
Since the libraries that are required by the platform are managed by a dedicated for this repository, Maven tool is required for building.
In order to build the test application, switch to its folder and run "build.sh" script, which contains the corresponding Maven command sequence.
You can also execute maven directly with the following commands: "mvn clean compile assembly:single"

## Running
The test application provides two examples of the application execution configuration - for 2 and 3 initial "maps".
They are provided in the corresponding *.xml files. For running them, please execute either of two run_*.sh scripts.
For a more complete description of the application model specification, please refer to JUNIPER deliverable D5.6 (available at www.juniper-project.eu).

## Development of new applications
We recommend using the Eclipse project supplied with the included MapReduce application.

## Support and Contact
You may contact us at cheptsov*at*hlrs.de for any further information on the JUNIPER platform or if any support is needed.