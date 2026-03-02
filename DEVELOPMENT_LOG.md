# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

# Development Log

---

## Entry 1 – [March 2, 2026 – 5:30 PM]

**What I did:**  
Updated my student ID and verified the project setup.

**Details:**  
- Modified the main file to include my correct student ID.  
- Checked that the project compiles successfully after the modification.  
- Reviewed the repository structure to make sure everything is organized properly.

**Challenges:**  
I was unsure where exactly my ID should be placed in the code.

**Solution:**  
I reviewed the assignment instructions carefully and confirmed the correct location before committing the changes.

**Time spent:** 30 minutes  

---

## Entry 2 – [March 3, 2026 – 6:15 PM]

**What I did:**  
Started implementing the Round-Robin scheduler structure.

**Details:**  
- Reviewed how Round-Robin scheduling works.  
- Implemented the ready queue using Queue<Thread>.  
- Used FIFO behavior with processQueue.poll().  
- Structured the main scheduling loop.

**Challenges:**  
I needed to clearly understand how threads simulate processes.

**Solution:**  
I revised how Thread.start() and Thread.join() work and applied them step by step inside the loop.

**Time spent:** 1 hour  

---

## Entry 3 – [March 4, 2026 – 7:30 PM]

**What I did:**  
Improved process execution logic and re-queuing behavior.

**Details:**  
- Used isFinished() to check if a process completed.  
- Re-added unfinished processes back into the ready queue using addProcessToQueue().  
- Verified fairness of Round-Robin scheduling.

**Challenges:**  
Processes were not behaving correctly when they didn’t finish within one quantum.

**Solution:**  
Adjusted the condition logic and tested multiple runs to ensure correct re-queuing.

**Time spent:** 1 hour  

---

## Entry 4 – [March 5, 2026 – 8:45 PM]

**What I did:**  
Implemented Feature 2 (Context Switch Counter).

**Details:**  
- Added a static variable contextSwitches.  
- Incremented it when switching between processes.  
- Printed the total context switches at the end of the simulation.

**Challenges:**  
I was unsure about the exact placement of the counter increment.

**Solution:**  
Placed it inside the scheduling loop before starting the next thread and ensured it increments only when appropriate.

**Time spent:** 45 minutes  

---

## Entry 5 – [March 6, 2026 – 9:45 PM]

**What I did:**  
Implemented Feature 3 (Waiting Time Tracking).

**Details:**  
- Added createdTime, lastEnqueueTime, and totalWaitingTime to the Process class.  
- Updated lastEnqueueTime inside addProcessToQueue().  
- Calculated waiting time before process execution.  
- Printed waiting time summary at the end.

**Challenges:**  
Waiting time calculation was incorrect at first because enqueue time was not updated properly.

**Solution:**  
Moved the waiting time calculation to the correct location and verified the logic step by step.

**Time spent:** 1 hour  

---

## Summary

**Total time spent on assignment:** Approximately 4 hours and 15 minutes  

**Most challenging part:**  
Determining the correct placement for context switch counting and waiting time calculation.

**Most valuable learning:**  
Understanding how Round-Robin scheduling ensures fairness between processes and how thread management simulates CPU scheduling.

**What I would improve next time:**  
Plan the structure of the scheduler before coding to avoid repositioning logic multiple times.
