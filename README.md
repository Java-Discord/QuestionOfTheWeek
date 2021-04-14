
# Question-of-the-Week
Questions and answers of all QOTW starting 28.03.2021 - This includes all answers, including wrong ones

## What is QOTW?
QOTW, or Question of the week, is a weekly java-related question you can answer and be awarded points for. Check it out in `#question-of-the-week` on the [Java Discord](javadiscord.net).

## Questions/Answers

 - [Week 21 (21.03.2021 - 28.03.2021)](#week21)  
 - [Week 22 (28.03.2021 - 04.04.2021)](#week22)
 - [Week 23 (05.04.2021 - 11.04.2021)](#week23)
 - [Week 24 (11.04.2021 - 18.04.2021)](#week24)

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

---

<a name="week22"></a>
### Week 22 (28.03.2021 - 04.04.2021) | What are the main differences between Array and Collection?

 - Submission by dan1st#7327

[Arrays are a language feature that allows to store multiple elements of the same type (any type is allowed) in memory. Arrays have a fixed length.](https://docs.oracle.com/javase/specs/jls/se15/html/jls-10.html)
[`Collection`](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/util/Collection.html) is an general purpose interface for data structures. It is part of the standard library and not part of the language itself. It is also not possible to just create a collection but only to create instances of concrete implementations of `Collection`.

An example of a Collection is ArrayList. ArrayList is a concrete List (special form of s collection) that uses arrays internally. ArrayList starts with no elements (by default) and allows to add elements at any point (the internal array id recreared when needed). While there is only a single array implementation, there a many different Collections for different purposes. Most of them have a variable length, some have a fixed/maximum length.

 - Submission by Spider EveryOS#8098

An array is a fixed-length data type which allows you to hold many objects.
A collection is a class that can be either fixed-length or variable-length. It also holds objects, but does so in a different way depending on the type of collection. For example, maps have both an index key and a value.
The syntactic method of accessing the two is different. Arrays can be indexed with the `[i]` syntax, while Collections are often indexed with getters, setters, and other auxiliary methods.

 - Submission by Andrew.#3939

Arrays are a fixed-size, contiguous block of memory that is allocated for storing primitives or objects, whereas the Java Collections Framework is a layer of abstraction that provides programmers with a set of pre-implemented data structures, some of which use arrays as their internal data storage medium. Arrays have a special bracket-syntax for accessing and setting the value of variables at specific points in the array, using integer indexes starting from zero and going to the size of the array - 1, whereas collections offer methods for data access instead. Generally, collections use more memory, but offer more functionality than arrays for the average developer.

 - Submission by Dioxin#9863

Arrays are low-level data structures, while collections are high-level data structures.

Although both are objects in Java, collections provide a more functional interface: you can `sort`, you can `clear()`, and you can query active elements using `size()` (which differs from array's `length`, which queries the fixed-size of the array).

Some of the functions that make collections more functional than arrays are `add`, `remove`, and `contains`.

---

<a name="week23"></a>
### Week 23 (05.04.2021 - 11.04.2021) | What is the difference between ScheduledExecutorService and ExecutorService interface?

 - Submission by dan1st#7327

`ExecutorService` is an interface that allows to run tasks asynchronously. The utility class `Executors` provides various methods for obtaining `ExecutorService`s.
`ScheduledExecutorService` is another interface that extends `ExecutorService`. It does not only allow to run tasks but it allows to run tasks after a specific amount of time passes or periodically. Objects of `ScheduledExecutorService` can also be executed using `Executors`, especially using `Executors.newScheduledThreadPool()` or similar.

 - Submission by Dioxin#9863

*due to the immense formatting I will just put a picture here*
![image of submission by Dioxin#9863](https://user-images.githubusercontent.com/66334318/114774615-a8462780-9d70-11eb-9b66-73d900f612ba.png)

 - Submission by Ike#2932
 
*this did not score a point btw*

One is scheduled and one is not

 - Submission by Spider EveryOS#8098

*Dynxsty thought about not counting this but decided to*

The scheduled version of the executor has a specified delay before the thread for the task is started.

---

<a name="week24"></a>
### Week 24 (11.04.2021 - 18.04.2021) | What is Encapsulation?

-Submission not closed yet-



