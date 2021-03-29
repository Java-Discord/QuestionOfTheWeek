
# Question-of-the-Week
Questions and answers of all QOTW starting 28.03.2021

## What is QOTW?
QOTW, or Question of the week, is a weekly java-related question you can answer and be awarded points for. Check it out in `#question-of-the-week` on the [Java Discord](javadiscord.net).

## Questions/Answers

 - [Week 21 (21.03.2021 - 28.03.2021)](#week21)  
 - [Week 22 (28.03.2021 - 04.04.2021)](#week22)

<a name="week21"></a>
### Week 21 (21.03.2021 - 28.03.2021) | What are the advantages of multithreading?

 - Submission by dan1st#7327

Singlethreaded programs can only execute one thing at a time. If multiple operations should be executed in parallel, it would be required to check for other operations constantly. If the thread blocks (because of e.g. I/O or a loop), the whole program blocks. This makes asynchronous I/O the only option for I/O operations with a single thread as the program cannot execute other operations while waiting for I/O. Also, multiple threads cab utilize multiple CPU cores and therefore speed up computations. This is very well described in the book `Java Concurrency in Practice`.

 - Submission by Spider EveryOS#8098

Threading takes advantages of the OS's scheduling processes and allows you to make multiple tasks appear as if they were running concurrently. Additionally, on systems with multiple cores, multi-threading may allow programs to leverage the power of multiple cores at once.

 - Submission by OneWholesomeDev#7465

Multithreading allows making use of simultaneous calculations and operations. Which means in certain cases and when used correctly, you may get better performance off a certain process or algorithm. Thus you can split the possible bottlenecking 100 % load for one thread down to multiple 40 % load-threads. - Can be faster - No bottleneck

 - Submission by AttilaTheHun#9489

Multithre_ding_ allows us to run numerous task simultaneously, which is extra useful when you need several tasks running at the same time, or when you are doing some blocking operations. However it is good to keep in mind that working with multiple threads can lead to some unexpected behavior, mainly if the threads are accessing the same resources. Multithreading is also used in brute-force algorithms to check all the cases in a shorter time, making them much more powerful.

<a name="week22"></a>
### Week 22 (28.03.2021 - 04.04.2021) | What are the main differences between Array and Collection?

-Answers still open-
