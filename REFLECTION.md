# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

From this assignment, I learned how multithreading works in practice rather than just theory. I understood how each thread can simulate a process in a CPU scheduling system. Using Thread.start() and Thread.join() helped me see how execution flow is controlled between different threads. I also learned how context switching happens when the CPU moves from one process to another. Implementing Round-Robin scheduling helped me understand fairness and time quantum in a deeper way. Before this assignment, these concepts felt abstract, but now I can see how they are applied in real code.
---

## Question 2: What was the most challenging part of this assignment?
The most challenging part of this assignment was implementing the waiting time calculation correctly. At first, I placed the waiting time logic in the wrong position inside the loop, which caused incorrect values. I also struggled with understanding exactly when to increment the context switch counter. Since scheduling depends on correct execution order, small mistakes affected the final output. It was difficult because the logic looked correct at first glance, but the results were not accurate. This made me realize how sensitive scheduling algorithms are to small implementation details.


---

## Question 3: How did you overcome the challenges you faced?
I overcame the challenges by debugging step by step and testing the program multiple times. I carefully traced the execution flow of the scheduler and printed intermediate results to understand what was happening. I also reviewed the lecture slides to confirm the expected behavior of Round-Robin scheduling. Breaking the problem into smaller parts helped me focus on one issue at a time. Instead of rewriting everything, I adjusted the placement of specific lines like the waiting time calculation. This systematic approach helped me fix the errors and understand the logic better.

---

## Question 4: How can you apply multithreading concepts in real-world applications?
Multithreading concepts can be applied in many real-world applications such as web servers, games, and mobile apps. For example, a web server handles multiple client requests simultaneously using threads. In games, different threads may manage graphics, physics, and background tasks at the same time. In mobile apps, threads allow the user interface to remain responsive while background tasks run. The Round-Robin concept ensures fairness, similar to how systems share CPU time between applications. This assignment helped me understand how scheduling improves responsiveness and fairness in real systems.


---

## Additional Reflections (Optional)

### What would you like to learn more about?

---

### How confident do you feel about multithreading concepts now?



### Feedback on the assignment

