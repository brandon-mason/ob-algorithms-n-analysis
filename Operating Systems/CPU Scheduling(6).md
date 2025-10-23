 OS's optimize CPU usage by "context switching." This means that when one process is waiting or its execution is blocked, the OS takes the CPU from that process and moves it to another so that no CPU time is wasted.
This is achieved through holding many processes in memory at the same time.

<hr>
## CPU-I/O burst cycle
Processes start on CPU burst and the alternate between the two until the system requests that the process terminates.
![[Pasted image 20250915185610.png]]

<hr>
## CPU Scheduling Decisions
Decisions are made when...
1. the process switch from running to blocked.
2. the process switch from running to ready.
3. a new process arrives.
4. the process terminates.
5. the process switch from blocked to ready.
A new process must be chosen to execute after 1 and 4.

### Non-Preemptive Scheduling
- Occurs under situation 1 or 4.
- There is only one option for what to do.
### Preemptive Scheduling
- Running processes can be interrupted and placed in the ready queue.
- Has greater overhead but better services.
- Example interrupts:
	- Timer Interrupt
	- New process arrives.
	- Process goes from blocked to ready.

<hr>
## Work-conserving
CPU can’t go idle while a process is ready.
## Non-work conserving
Predictability

## Evaluating different scheduling algorithms
1. Throughput
	- Processes done per unit of time
2. Turnaround time
	- Time from arrival to completion(how long it takes to complete the process)
3. CPU Utilization
	- Percent of time the CPU is busy
4. Waiting time
	- Time spent in the ready queue

<hr>
## Scheduling Algorithms
### First come first served
- Non preemptive(CPU keeps process until it releases the CPU, i.e. terminating or switching to I/O burst)
- Advantages:
	- If service times are known then a process knows when it will complete.
- Disadvantages:
	- Fair
	- Simple
	- Long average wait time.
### Shortest Job First
- Non preemptive
- Assign CPU to the process with the shortest CPU burst.