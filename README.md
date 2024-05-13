# Parallel-Matrix-Operations-using-Threads-in-C

Welcome to the **Parallel Matrix Operations Suite**, a comprehensive collection of multi-threaded applications designed for efficient data handling and processing on a 2D matrix. Developed in C using POSIX threads (pthreads), this suite showcases advanced matrix operations using various data distribution strategies to maximize parallel performance on modern multi-core processors.

## Features

Our suite includes six distinct pthread applications, each tailored to execute one of three fundamental matrix operations—sum of rows, columns, or all elements—across different data distribution schemes:
- **Row-wise Block Distribution**
- **Column-wise Block Distribution**
- **Combined Row and Column-wise Block Distribution**
- **Row-wise Cyclic Distribution**
- **Column-wise Cyclic Distribution**
- **Combined Row and Column-wise Cyclic Distribution**

These applications utilize a standard 2D matrix of size `1024x1024` with integer elements, ensuring robust handling of large datasets.

## Technical Highlights

- **Multi-threaded Execution**: Leverages four parallel threads to enhance computational speed and efficiency.
- **Versatile Data Distributions**: Implements both block and cyclic distribution methods to optimize load balancing and minimize thread idle time.
- **Accuracy Validation**: Includes a `bool CorrectOutputCheck()` function to ensure that outputs from multi-threaded operations are consistent with those produced by serial algorithms.
- **Separate Buffering**: Utilizes a dedicated buffer for data distribution, avoiding common pitfalls associated with direct manipulation of matrix indices.

## Application Selection

The choice of matrix operations (sum of rows, columns, or all elements) for each pthread application was carefully made to best demonstrate the advantages of different distribution strategies in real-world scenarios, ensuring that each implementation showcases optimal data handling and computational efficiency.

## Getting Started

To begin using the Parallel Matrix Operations Suite, clone this repository and compile the code using your preferred C compiler with support for POSIX threads. Run each application with the provided makefile commands to see the power of parallel processing in action.

## Build Instructions

```bash
gcc -pthread -o matrix_operations1 matrix_operations1.c
./matrix_operations1
```

## Contributing
Interested in contributing? We welcome enhancements, bug fixes, and optimizations. Please send me a pull request or open an issue to discuss your ideas. If there's anything else you'd like to know about it, let me know. Feel free to reach me out at Maryamkhalid590@gmail.com

## License
This project is licensed under the MIT License - see the LICENSE file for details.

