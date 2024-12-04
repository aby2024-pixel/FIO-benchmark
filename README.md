# FIO-benchmark

ATC/OSDI '23 Tutorial: Simple FIO Benchmark
This repository contains my contributions to the ATC/OSDI '23 Tutorial Simple FIO Benchmark project. This artifact is part of Trovi on the Chameleon Cloud platform. My contributions aim to enhance or extend the functionality of the existing project.

Here is a template for your GitHub README file tailored to the "ATC/OSDI 23 Tutorial Simple FIO Benchmark" project. It provides clear instructions and information for your professor to follow:

ATC/OSDI '23 Tutorial: Simple FIO Benchmark
This repository contains my contributions to the ATC/OSDI '23 Tutorial Simple FIO Benchmark project. This artifact is part of Trovi on the Chameleon Cloud platform. My contributions aim to enhance or extend the functionality of the existing project.

Table of Contents
Project Overview
Contributions
Getting Started
Setup Instructions
Running the Benchmark
Results and Analysis
Acknowledgments

Project Overview
The Simple FIO Benchmark is a tool designed to perform input/output operations benchmarking for storage devices. It is an artifact associated with the ATC/OSDI '23 Tutorial series, hosted on the Chameleon Cloud platform.

This repository provides:

My contributions and modifications.
Setup and usage instructions

Contributions
Enhancements and Features Added
Automated FIO Benchmarking

Added a Python script to run FIO benchmarks programmatically using the subprocess module.
Sample command used: Random write operations with 4k block size, 2MB total size, single thread, and a runtime of 30 seconds.
Output processing and raw results are displayed for better usability.
Code Reference​1 [FIO_Output]
.
Operations Per Second, Throughput, and Latency Visualization

Implemented a script to parse and visualize Sysbench output.
Metrics include file operations (reads/s, writes/s, fsyncs/s), throughput (read/write in MiB/s), and latency (min, avg, max).
Generated bar charts and line graphs for clear representation.
[Code Reference] (operations per second,throughput,latency.txt)​2
.
SSD vs. RAM Disk Performance Analysis

Developed a detailed performance analysis script comparing SSDs and RAM disks.
Features include:
Visualization of performance trends with average performance overlays.
Variability analysis using standard deviation.
Enhanced logging for traceability.
[Code Reference](performance of SDD and Ram Disk.txt)​3
.
Sysbench Benchmark Automation

Automated the following Sysbench benchmarking tasks:
Cleanup of old test files.
Preparation of new test files (1GB total size, split into 128 files).
Execution of CPU and memory benchmarks with multi-threading.
Cleanup post-benchmark for resource management.
Incorporated error handling for better reliability.
Code Reference​4 [sysbench]
.
These contributions aim to improve benchmarking automation, data analysis, and visualization, offering a comprehensive evaluation of system performance. Each enhancement is designed to simplify execution and interpretation of results for the end user.

Getting Started
Prerequisites
To run this project, you will need:

Chameleon Cloud Access: Set up an account on Chameleon Cloud.
Trovi Access: Ensure the artifact is accessible from Trovi.

Once you get access to Trovi, type FIO in the search bar and press enter.
look for this "ATC/OSDI 23 Tutorial Simple FIO Benchmark".

click on it and once you get to the page, click on Launch Chameleon.
you will get to the existing code. Then in the contributions part, click on any file stored in my main file to get access to the code . Once you are there, copy the code from any file and paste in the jupyter notebook where the project is. Before that I want to make sure that some steps need to be done. Here are the steps:

Installing FIO

sudo apt-get update
sudo apt-get install fio

Installing sysbench

sudo apt update
sudo apt install -y sysbench
sysbench --version

Results and Analysis
The output results will be shown as you execute the code. 
 
