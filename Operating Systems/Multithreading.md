## Benefits
##### Responsiveness
Allows the program to perform lengthy processes without blocking the main thread
##### Resource Sharing
Processes share resources through certain techniques(**written in a different note**). 
Threads share resources of the process they belong to which allows for a process to have multiple threads running concurrently.
##### Economy
Explicitly allocating memory and resources for process creation is costly. With threads, the OS can **context-switch** threads, meaning a thread will be transferred to another process that wants to perform the operation the thread was already doing. This avoids having to reallocate address space in the memory, which is a costly operation.
##### Scalability
Gets even more beneficial in multiprocessor architecture.

<hr>
## Multicore Programming
### Concurrency vs Parallelism
##### Concurrency
All threads make progress by running for a short period of time on a single processing core.
##### Parallelism
Two threads run at the same time, each getting their own core.

### Challenges
##### Identifying tasks
Applications need to be examined to find areas, that can be divided into separate tasks that can run concurrently. Ideally they run independent of one another so they can be on their own cores.
##### Balance
Tasks should perform equal work of equal value. This is to prevent a non costly task from taking up a whole core.
##### Data splitting
Data accessed and manipulated by tasks must be divided between cores as well.
##### Data dependency
Tasks must be synchronized so that when one task depends on data from another, the dependent task doesn’t get blocked.
##### Testing and debugging
Multiple different execution paths are possible when running on multiple cores making testing more difficult.

<hr>
## Amdahl's Law
