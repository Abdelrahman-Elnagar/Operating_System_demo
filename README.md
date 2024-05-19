# OS Scheduler Project

## Overview

Welcome to the OS Scheduler Project! This project simulates the scheduling of processes in an operating system using two different scheduling algorithms: Shortest Job First (SJF) and Round Robin (RR). The primary goal of this project is to demonstrate process scheduling and memory management in a simple, educational context.

## Features

- **Process Management**: Create and manage processes with instructions read from text files.
- **Memory Management**: Allocate and manage memory for each process.
- **Scheduling Algorithms**:
  - **Shortest Job First (SJF)**: Prioritizes processes with the shortest burst time.
  - **Round Robin (RR)**: Uses time slicing to switch between processes.
- **Execution Simulation**: Simulate the execution of processes and generate Gantt charts for visualization.

## Project Structure

The project is organized into several classes, each with specific responsibilities:

- **Process**: Represents a process with its instructions and PCB (Process Control Block).
- **PCB**: Holds process-specific information like ID, program counter, base, and limit registers.
- **Memory**: Manages memory allocation and variable storage for processes.
- **ReadyQueue**: A queue to hold processes that are ready to be executed.
- **Scheduler**: An interface for scheduling algorithms.
- **RoundRobin**: Implements the Round Robin scheduling algorithm.
- **SJF**: Implements the Shortest Job First scheduling algorithm.
- **Execution**: Handles the execution of processes and the generation of Gantt charts.
- **Main**: Entry point of the program, manages user interaction and starts the scheduling simulation.

## Installation and Usage

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- A terminal or command prompt

### Running the Program

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/OS-Scheduler.git
    cd OS-Scheduler
    ```

2. **Compile the source files**:
    ```sh
    javac -d bin src/OS/*.java
    ```

3. **Run the program**:
    ```sh
    java -cp bin OS.Main
    ```

### User Interaction

When the program starts, you will be prompted to:
1. Enter the number of process files.
2. Enter the file paths for each process.
3. Choose a scheduling algorithm (SJF or RR).

The program will then simulate the scheduling and execution of processes, displaying the state of memory and generating a Gantt chart for visualization.

## Contributing

We welcome contributions to improve this project. Please fork the repository and submit pull requests with your changes. Make sure to follow the existing coding style and document your code appropriately.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or suggestions, feel free to open an issue in the repository or contact the maintainer at [your.email@example.com](mailto:abdelrahmanelnagar123@gmail.com).

## Acknowledgements

This project was inspired by the need to provide a simple yet comprehensive example of process scheduling and memory management in an educational setting. We hope this project helps students and enthusiasts understand the basics of these crucial operating system concepts.

## Example Process File Format

Each process file should contain instructions in the following format:
```bash
assign x input
assign y readFile path/to/file
assign z add x y
writeFile path/to/output/file z
print z
```

## Future Enhancements

- **Additional Scheduling Algorithms**: Implementing more scheduling algorithms like Priority Scheduling and Multilevel Queue Scheduling.
- **Graphical User Interface (GUI)**: Adding a GUI for better visualization and interaction.
- **Error Handling**: Improving error handling and user feedback.

---

Thank you for using the OS Scheduler Project! We hope it serves as a valuable learning tool and a solid foundation for further exploration into operating systems and process management.

