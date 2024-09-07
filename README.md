# CPU Scheduling Algorithms

**CPU Scheduling Algorithms** are methods used by operating systems to manage and prioritize the execution of processes in a computer system. Below is a brief overview of some commonly used CPU scheduling algorithms:

### 1. First-Come, First-Served (FCFS)
- Processes are executed in the order they arrive in the ready queue.
- Simple and easy to implement.
- May lead to poor average waiting times, especially for long processes that arrive first (convoy effect).

### 2. Shortest Job First (SJF)
- Selects the process with the smallest execution time next.
- Reduces average waiting time compared to FCFS.
- Requires knowing the execution time of each process in advance or estimating it accurately.

### 3. Shortest Remaining Time First (SRTF)
- A preemptive version of SJF.
- If a new process arrives with a shorter burst time than the currently running process, it preempts the current process and starts executing immediately.
- Minimizes the average waiting time by prioritizing short processes.

### 4. Longest Job First (LJF)
- Opposite of SJF, prioritizes longer processes.
- Not commonly used due to its tendency to cause long waiting times for short processes.

### 5. Priority Scheduling
- Each process is assigned a priority, and the scheduler selects the process with the highest priority for execution.
- Can be either preemptive or non-preemptive.
- May suffer from starvation if lower-priority processes never get a chance to execute.

### 6. Round Robin (RR)
- Each process is assigned a fixed time slice (quantum), and the scheduler rotates between processes, executing each for a time quantum.
- Preemptive and ensures fairness among processes.
- Can lead to higher context switching overhead, especially with small time slices.
- Well-suited for time-sharing systems and interactive environments.

These algorithms vary in terms of their efficiency, fairness, and complexity. The choice of scheduling algorithm depends on the specific requirements and characteristics of the system.

---

## About the Project

This project implements different scheduling algorithms based on user input. Users can select the scheduling algorithm they want to execute, and then input the number of processes, arrival time, and burst time accordingly. The output is displayed in a table format, showing the following for each process:
- **Completion Time**
- **Turnaround Time**
- **Waiting Time**

Finally, the **average Turnaround Time** and **average Waiting Time** are calculated and displayed.
