# Airport Baggage Handling and Sorting Simulator

**NAME:** ADEENA AIEESYA BINTI AHMAD SHUKRE

**STUDENT ID:** 2024648084

**CLASS:** M3CS2554A

-------------------------------------------------------------------------------------------


## INTRODUCTION 
The foundation of a good airport operation is effective baggage handling and sorting system, which guarantee seamless traveler experiences and efficient logistics. In modern airports, thousands of baggage items must be processed, sorted, and delivered accurately within time frame. Any mistakes in the process can lead to delays, misplaced luggage, and passenger frustration. As air travel continues to grow, the need for faster and more efficient baggage processing systems becomes increasingly important.

Traditionally, many systems rely on sequential programming, where tasks are executed one at a time. Although this method is straightforward, it becomes ineffective when managing massive amount of data, especially in situations where multiple tasks take place at the same time. In real world environments, baggage arrives from multiple check-in counters at the same time, requiring systems that can handle concurrent inputs and perform quick sorting operations.

To overcome this issue, concurrency and parallelism are introduced in modern computing. Concurrent programming allows several tasks to be managed at once, improving system responsiveness, while parallel programming allows tasks to be executed simultaneously across various CPU cores, improving performance for computationally demanding workloads.



## PROBLEM STATEMENT
In the context of airport baggage handling, where thousands or even millions of records may need to be processed, selecting the most efficient processing method becomes critical.

While the sequential processing provides a simple approach, it may not be suitable for handling large volumes of data efficiently. At the same time, concurrent and parallel techniques offer potential performance improvements, but their effectiveness depends on how they are implemented and the nature of the workload.

Thus, this project focuses on evaluating and comparing three processing techniques, which are sequential, concurrent, and parallel processing by simulating a large scale airport baggage handling system. The aim is to identify which approach provides better performance and scalability when handling large datasets.



## OBJECTIVES
The main objective of this project is to design and develop an airport baggage handling and sorting simulator using Python to model the processing of large scale baggage data. The system aims to simulate real world scenarios by automatically generating a large number of baggage records and processing them using different execution techniques.

Other than that, this project aims to implement and evaluate three different processing approaches, which are sequential programming as a start, concurrent processing using threding to handle multiple tasks simultaneously, and parallel processing using multiprocessing to make use of various CPU cores.

Also, the project focuses on comparing the performance of these approaches by measuring execution time and efficiency when processing huge datasets, including data sizes in the range of hundreds of thousands to millions of records. Through this comparison, the project intends to identify the most suitable technique for large scale data processing and to demonstrate the practical benefits of concurrency and parallelism in improving system performance.



## SYSTEM DESIGN
This project follows a simulation based approach to model airport baggage handling using different processing techniques. The system is designed to generate a massive number of baggage records and process them using sequential, concurrent, and parallel methods.

First, the system generates baggage data automatically based on user input. Each baggage record contain basic information such as bag ID, weight, destination, priority, and complexity level. The use of automatically generated data allows the system to simulate large scale situations without requiring manual input.

Next, the system processes the generated data using three different techniques. In sequential processing, each baggage record is processed one by one. In concurrent processing, multiple threads are used to process baggage records simultaneously by retrieving tasks from a shared queue. In parallel processing, multiple processes are created using a process pool, where each process handles part of the workload independently.

The system measures the execution time for each processing method using a timer. This allows a direct comparison of performance between the three approaches. After processing is complete, the system displays a summary of results, including the number of baggage items processed and the total workload score.




## IMPLEMENTATION
The system is implemented in Python and is structured into several functions where each function is responsible for a specific part of the program. The implementation focuses on generating huge scale data and processing it using three different techniques, which are sequential, concurrent, and parallel processing.

The program begins with data generation function, which automatically creates a great amount of baggage records based on user input. Each record is stored as a tuple containing values such as bag ID, weight, destination index, priority index, and complexity level. Using a tuple helps reduce memory usage, making it suitable for handling big datasets.

Next, the sorting workload function is used to simulate the processing of each baggage item. This function performs repeated calculations based on a complexity value to represent a CPU operation. The purpose of this function is to create a measurable workload so that performance differences between processing techniques can be observed.

For sequential processing, the program uses a simple loop to process each baggage record one at a time. This method serves as a baseline for comparison, as it does not involve any form of concurrency or parallelism.

For concurrent processing, the program uses Python’s threading module. A shared queue is used to store all baggage tasks, and multiple threads are created to retrieve and process tasks from this queue. A lock mechanism is used to ensure that shared data, such as result counters, is updated safely without causing conflicts between threads.

For parallel processing, the program uses the multiprocessing module. A process pool is created to distribute tasks across multiple processes, allowing them to run simultaneously on different CPU cores. The map function is used to assign tasks to processes efficiently, and a chunk size is specified to improve performance when handling large datasets.

The program also includes a timing mechanism using a high-resolution timer to measure the execution time for each processing method. This allows for an accurate comparison of performance between sequential, concurrent, and parallel approaches.

Finally, the program summarizes the results by counting the number of baggage items processed for each destination and calculating the total workload score. This summary is displayed along with execution time, giving a clear comparison of how each technique performs under the same condition.



## RESULTS AND DISCUSSION



