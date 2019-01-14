# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > *Concurrency is running multiple tasks at what seems like the same time, here the tasks are not necessarily finished before moving on to the next task. Parallelism is when multiple tasks are actually being run at the same time by using multi-core CPU. The difference is that concurency seemingly rund multiple tasks at the same time, while parallellism actually runs multiple tasks at the same time*
 
 ### Why have machines become increasingly multicore in the past decade?
 > * It's easier to make the machines better by using several cores than it is to always make better single-core CPU. Which means that development of better machines is faster and better by using multy core CPU. Another reason is that by runing tasks in parallell, which can be done with multi core, the performance of the machine will increase.*
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > *Problems that do not need a lot of process power, but have a long waiting time, then it's possible to go to another task/problem while the other one is waiting*
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *They make a programmer's life harder*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > *Processes is the program that is being executed. Threads is parts of the process which is started by the operating system. Green threads is threads started by a virtual machine. Coroutines is that all threads that shares a processor decides how long time is needed before another thread can "use" the processor*
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *They create green threads*
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *GIL prevents multiple threads from runing at the same time, concurrency*
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *CPython*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *Changes the maximum of processors that can be used to execute a task*
