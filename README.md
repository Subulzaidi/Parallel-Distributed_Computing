# Python Basics and Advanced Programming Examples

This repository contains a collection of Python programs designed to help you learn a wide range of programming techniques, from fundamental concepts to advanced topics. The examples include basic arithmetic operations, object-oriented programming (OOP), and more complex topics such as parallel computing, threading, multiprocessing, GPU utilization, and asynchronous programming. Whether you are a beginner or an intermediate developer, these scripts will guide you through key Python programming concepts and advanced features.

## Table of Contents

1. [Overview](#overview)
2. [Script Descriptions](#script-descriptions)
3. [Installation](#installation)
4. [Prerequisites](#prerequisites)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)

## Overview

This repository is structured into different chapters that focus on various aspects of Python programming. Each script is designed to help you understand different concepts, tools, and libraries that Python offers for both simple and complex tasks. From basic arithmetic calculations to managing processes using Python’s `multiprocessing` module, this collection covers a variety of programming techniques.

### Key Topics Covered:
- Basic programming concepts such as functions, data structures, and classes.
- Object-oriented programming (OOP) in Python.
- Advanced parallel computing techniques, including the use of multiprocessing, threading, and GPU.
- Inter-process communication methods and synchronization techniques for multi-core and multi-threaded environments.
- Asynchronous programming with asyncio and concurrent futures.

## Script Descriptions

### 1. **calculator.py**  
A simple calculator program that allows users to perform basic arithmetic operations:  
- Addition  
- Subtraction  
- Multiplication  
- Division  
Users input two numbers and select the operation to get the result.

### 2. **data_structures.py**  
This script provides examples of Python's core data structures, including:  
- Tuples  
- Lists  
- Dictionaries  
You will learn how to use them effectively in various scenarios.

### 3. **functions.py**  
A guide to creating and using functions in Python, including:  
- Function definitions  
- Parameters and return values  
- Calling functions with different arguments  

### 4. **classes.py**  
Introduces object-oriented programming (OOP) in Python:  
- Defining classes and creating objects  
- Writing methods  
- Demonstrating inheritance to reuse and extend code  

### 5. **mpi_example.py**  
Explains how to perform distributed computing using the **MPI** library (`mpi4py`):  
- Sending and receiving messages between processes  
- Understanding process ranks and sizes in MPI contexts  

### 6. **multiprocessing_vs_threading.py**  
A comparative script that explains the differences between multiprocessing and threading:  
- **Multiprocessing**: Runs tasks in separate processes to utilize multiple CPUs.  
- **Multithreading**: Shares memory space between threads for concurrent execution.  
Performance differences are analyzed through a basic list-processing task.

### 7. **gpu_computation.py**  
Showcases how to accelerate computations using **Numba's CUDA JIT**:  
- Implements vector addition on a GPU for performance gains.  
- Includes result validation using Numba’s CUDA functionality.

### 8. **num_parallel_computing.py**  
Demonstrates data parallelism with **NumPy**:  
- Performs vector addition using NumPy’s optimized array operations.  
- Measures execution times for large-scale computations.

### 9. **threadpool_executor.py**  
Explores task parallelism using `ThreadPoolExecutor`:  
- Manages a pool of threads to execute functions concurrently.  
- Executes tasks asynchronously, simplifying thread management.

### 10. **producer_consumer.py**  
Illustrates the classic producer-consumer problem using Python's **multiprocessing** module:  
- A `producer` generates items and adds them to a shared queue.  
- A `consumer` retrieves and processes items from the queue.

### 11. **semaphore_example.py**  
Demonstrates the use of **semaphores** in threading to limit access to shared resources:  
- Controls the number of threads accessing a resource concurrently.

### 12. **multiprocessing_example.py**  
Explains the basics of Python’s **multiprocessing** module:  
- Runs two separate functions (e.g., square and cube calculations) in parallel.  
- Includes process synchronization and joining.

### 13. **fibonacci_threading.py**  
Calculates Fibonacci numbers using **multithreading**:  
- Distributes computation across multiple threads to improve efficiency.  

### 14. **threading_event_example.py**  
Uses threading events for inter-thread communication:  
- A producer thread generates random numbers.  
- A consumer thread processes them, synchronized using an event.

### 15. **lock_example.py**  
Explains the use of thread locks for synchronization:  
- Prevents race conditions by ensuring only one thread accesses a shared resource at a time.

### 16. **Process-Based Parallelism**  
In this chapter, we cover advanced multiprocessing techniques, including:  
- **communicatingWithPipe**: Inter-process communication using pipes for data exchange.  
- **communicatingWithQueue**: Sharing data between processes using a thread-safe queue.  
- **killingProcesses**: Terminating processes gracefully.  
- **namingProcess**: Assigning names to processes for easier identification.  
- **runBackgroundProcesses**: Running processes in the background while the main program continues.  
- **spawningProcess**: Spawning new processes dynamically to execute tasks concurrently.

### 17. **Message Passing**  
Chapter 5 focuses on message-passing techniques to enable efficient communication between processes, including:  
- **broadcast**: Sending messages from one process to all other processes simultaneously.  
- **deadLockProblems**: Understanding and preventing deadlocks when multiple processes are waiting for resources.  
- **pointToPointCommunication**: Facilitating communication between two specific processes.  
- **gather**: Collecting data from multiple processes into one process.  
- **scatter**: Distributing data from one process to multiple processes.

### 18. **Asynchronous Programming**  
Chapter 6 covers asynchronous programming using Python’s `asyncio` library and `concurrent.futures`. Key topics include:  
- **asyncioAndFuture**: Using `asyncio` in conjunction with `Future` objects to manage asynchronous tasks and future results.  
- **asyncioCoroutine**: Implementing coroutines to execute asynchronous tasks concurrently.  
- **asyncioEventLoop**: Understanding the role of the event loop in managing asynchronous tasks.  
- **concurrent_futures_pooling**: Utilizing `concurrent.futures` to manage a pool of threads or processes for asynchronous task execution.  

## Installation

To run the scripts, you need Python 3.x installed on your system. Additionally, some scripts require external libraries.

### Install the required libraries using the following command:

```bash
pip install mpi4py numba numpy
