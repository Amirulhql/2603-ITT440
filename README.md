# Solitaire Parallel Programming Simulator
- Name : 'Aina Maisarah bt Mohd Shuhaimi
- Student ID :2024230508
- Course code : ITT440

## Abstract
This project presents the development of a Python-based simulation program designed to compare the performance of sequential, concurrent, and parallel programming techniques. The application simulates a large volume of solitaire game outcomes using probabilistic models.  

The program implements threading as a concurrent technique and multiprocessing as a parallel technique. Performance is evaluated based on execution time when processing millions of simulated games. The results demonstrate that multiprocessing achieves the best performance for CPU-bound tasks, while threading is limited due to Python’s Global Interpreter Lock (GIL).  
## Introduction
With the advancement of multi-core processors, parallel programming has become essential for improving computational efficiency. Different programming techniques such as sequential execution, threading, and multiprocessing offer various levels of performance depending on the nature of the task.

This project aims to develop a simulation system that processes a large volume of data in the form of solitaire game outcomes. The program compares execution performance using three approaches:

- Sequential programming
- Concurrent programming (threading)
- Parallel programming (multiprocessing)
## Objectives

- To develop a Python program that simulates a large number of solitaire games
- To implement concurrent programming using threading
- To implement parallel programming using multiprocessing
- To compare execution performance between different techniques
- To analyze the effect of CPU cores on program efficiency
  
## System Requirements
- Operating System: Kali Linux
- Python Version: Python 3.8 or higher
- CPU: 4 cores
- RAM: Minimum 4GB

## Program Development

The developed application simulates solitaire games using predefined win probabilities. Each simulation represents a game outcome (win or loss), and millions of games are processed to evaluate performance.

The program generates a large volume of data by simulating between:  
- 10 million to 50 million game iterations  
Each game result is determined using a random probability function.

Sequential Programming  
- Executes tasks one by one
- Uses a single CPU core
- Serves as baseline performance

Concurrent Programming (Threading)  
- Uses multiple threads (4 threads based on system CPU)
- Allows tasks to run concurrently
- Limited by Python GIL → cannot achieve true parallelism

Parallel Programming (Multiprocessing)  
- Uses multiple processes (4 processes)
- Each process runs independently
- Utilizes all CPU cores effectively
- Achieves true parallel execution

## Program Execution

## Results

# User Manual System Requirements
- Kali Linux
- Python 3 installed

## Installation Steps
Step 1: Install Python
sudo apt update  
sudo apt install python3  

## How to Run the Program  
1. Open terminal  
2. Navigate to file location  
Run:
phyton ITT440.py

## Sample Input / Output

## Screenshots

## Source Code

## Conclusion
This project successfully demonstrates the differences between sequential, concurrent, and parallel programming.

Multiprocessing is proven to be the most efficient approach for handling large-scale computational tasks, while threading is less effective due to inherent limitations in Python.

The program fulfills all assignment requirements by processing a large volume of data and clearly demonstrating performance differences between execution methods.
