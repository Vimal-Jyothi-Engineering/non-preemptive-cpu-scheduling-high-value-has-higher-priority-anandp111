[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/Daf--GaW)
# Non-Preemptive Priority CPU Scheduling
## Description
This project implements Non-Preemptive Priority CPU Scheduling using the C programming language.
In this scheduling algorithm, the CPU is allocated to the process with the highest priority value among the processes that have already arrived in the ready queue. Once a process starts execution, it continues until completion (non-preemptive).
In this implementation, higher priority value indicates higher priority.

## Input Format
The program first reads the number of processes.
For each process the following information is provided:
PID Arrival_Time Burst_Time Priority
Example:
P1 0 5 2
Where:
PID → Process ID
Arrival Time (AT)→ Time at which process enters the ready queue
Burst Time (BT) → CPU execution time required by the process
Priority (PR) → Higher value indicates higher priority

## Sample Input
4
P1 0 5 2
P2 1 3 4
P3 2 4 3
P4 3 2 5

## Sample Output
Waiting Time:
P1 0
P2 6
P3 8
P4 2
Turnaround Time:
P1 5
P2 9
P3 12
P4 4
Average Waiting Time: 4.00
Average Turnaround Time: 7.50

## Compilation
gcc priority.c -o priority
## Execution
.\priority.exe

## Algorithm
1. Read the number of processes.
2. Read process ID, arrival time, burst time and priority.
3. At each time unit select the process:
   * that has arrived
   * that is not completed
   * with the highest priority.
4. Execute the selected process completely.
5. Calculate:
   * Completion Time (CT)
   * Turnaround Time (TAT = CT − AT)
   * Waiting Time (WT = TAT − BT)
6. Repeat until all processes are completed.


## Author
Name:Anand P
Roll Number:14
REG No:VML24AD027
Institution: Vimal Jyothi Engineering College
