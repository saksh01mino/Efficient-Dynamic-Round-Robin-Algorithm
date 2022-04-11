# About
Operating systems are resource managers. The resources managed by operating systems are hardware, storage units, input devices, output devices and data. Operating systems perform many functions such as implementing user interface, sharing hardware among users, facilitating input/output, accounting for resource usage, organizing data, etc.

Whenever CPU becomes idle, a waiting process from ready queue is selected and CPU is allocated to that. The performance of the scheduling algorithm mainly depends on CPU 
utilization, throughput, turnaround time, waiting time, response time, and context switch. In Round Robin a small unit of time is used which is called Time Quantum or Time slice. The CPU scheduler goes around the ready queueallocating the CPU to each process for a time interval up to1 time quantum. If a process’s CPU burst exceeds 1 time quantum, that process is pre-empt and is put back in the ready queue .If a new process arrives then it is added to the tail of the circular queue. RR provides better performance as compared to the others in case of a time sharing operating system.

# Objective
To design a new Dynamic Round Robin Algorithm for increasing the performance of the CPU by decreasing the average waiting time and minimizing the number of context switches.To make one scheduling algorithm of our own and compare its waiting and turnaround time with other algorithms already there. 

# Proposed Algorithm
Our algorithm has taken the logarithm of a value and multiply it with the sum of two other values. Now, the mean of a data is that value which represents the entire data set in one value and it is the mean with which each value in the data set can correspond itself to. The median is the middle-most value of the data. So, the mean and median are the measures of central tendency, it is these values which can give us a representative value for the entire data. Thus, we have taken the logarithm of the sum of mean and median of the burst time of the processes. Now this logarithm is multiplied by the sum of natural log of mean and median and the difference between the mean and lowest burst time.

                                     𝑥 = log(𝑚𝑒𝑎𝑛 + 𝑚𝑒𝑑𝑖𝑎𝑛) ∗ (ln(𝑚𝑒𝑎𝑛 + 𝑚𝑒𝑑𝑖𝑎𝑛) + (𝑚𝑒𝑎𝑛 − 𝑙𝑜𝑤𝑒𝑠𝑡 𝑏𝑢𝑟𝑠𝑡 𝑡𝑖𝑚𝑒))

Now, consider an equation:
                         𝒚 = 𝟏𝟔 𝒍𝒏(𝒙) + 𝟑1

We now compute the values of y for x=1 to x=10. The value of y increases with the increasing value of x, indicating that the graph will be increasing. At the same time, another trend is observed that the difference between the values of y for increasing x is decreasing. Example, the difference between the values of y for x=1 and x=4 is 22.18. But the difference between thevalues of y for x=7 and x=10 is only 5.71. This indicates that there is a decay in the rate of rise in our graph. The graph will be of increasing nature but the rate of increase will be decreasing with the increasing value of x.

![Graph](1.png)
