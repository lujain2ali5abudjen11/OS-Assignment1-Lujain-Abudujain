# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

A process is an independent program in execution with its own memory space and system resources. Each process has its own address space, which makes it heavier in terms of memory and creation overhead. A thread, on the other hand, is a smaller unit of execution that runs within a process and shares the same memory space with other threads in that process.

Threads are more lightweight and faster to create compared to processes. In this assignment, we used threads because all simulated processes needed to be managed inside one Java program using a shared ready queue. Using separate processes would require more system resources and complex inter-process communication. Threads made the Round-Robin scheduler simulation simpler and more efficient.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

In Round-Robin scheduling, if a process does not finish its burst time within the given time quantum, it is paused and placed at the end of the ready queue. This ensures fairness because each process gets equal CPU time in cycles. The scheduler then selects the next process in the queue.

For example, in my program output, when P1 used its full time quantum but still had remaining burst time, the output showed that it was re-added to the ready queue. Later, it ran again when its turn came back. This demonstrates how Round-Robin rotates processes to prevent starvation and ensure fairness among all processes.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

1. **New**: P1 is in the New state when the thread object is created but before the start() method is called.

2. **Runnable**: After calling start(), P1 enters the Runnable state and waits in the ready queue for CPU scheduling.

3. **Running**: P1 enters the Running state when the scheduler selects it and it begins executing for its assigned time quantum.

4. **Waiting**: In the simulation, P1 may conceptually enter a waiting-like state when it is paused after using its time quantum and waiting for its next turn in the ready queue.

5. **Terminated**: P1 enters the Terminated state once its burst time becomes zero and it finishes execution completely.

This lifecycle shows how a thread transitions through different states during execution in a scheduling simulation.

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

### Example 1: Web Server Handling Multiple Clients

**Description**: A web server may handle many client requests at the same time. Each request can be handled by a separate thread.

**Why Round-Robin works well here**: Round-Robin ensures that each client request gets CPU time fairly. No single request can monopolize the CPU. This improves responsiveness and ensures all users experience reasonable service time.

### Example 2: Operating System Time-Sharing Systems

**Description**: In a time-sharing operating system, multiple user programs run simultaneously.

**Why Round-Robin works well here**: The scheduler gives each program a fixed time quantum, switching between them rapidly. This creates the illusion of parallelism and ensures fairness. It prevents starvation and keeps the system responsive for all users.

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between processes and threads.
2. How Round-Robin scheduling ensures fairness.
3. Thread lifecycle and state transitions.
4. Practical applications of time-sharing scheduling.

**Concepts I need to study more:**
1. Advanced synchronization mechanisms between threads.
2. Handling race conditions and deadlocks in complex systems.**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
