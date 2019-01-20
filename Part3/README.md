# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency is when you make code that can run at the same time. Parallelism is when the code is running at the same time. ie. the ability to do a thing vs. actually doing so.
 
 ### Why have machines become increasingly multicore in the past decade?
 > its easier to have more cores than to make singe cores that can run at higher frequencies without running into heat problems or stability problems.
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Doing multiple things at the same time, in way thats easy to scale.
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Can be both; It might require a change in perspective. And if the problem can be easily seperated into smaller problems. 
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > a process can have multiple threads. different processes dont share address space.
threads share address space.
Green threads are threads made by a vm or a runtime library instead of the operating system.

 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > `pthread_create()`  (C/POSIX) : thread.
 `threading.Thread()` (Python) : thread.
 `go` (Go) : green thread.
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > only one thread per process can run at a time
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Your answer here*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > it limits the amount of operating system threads that can run go user code at the same time.
