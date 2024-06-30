# RR
Program Explanation

1. Ask the user for number of processes n.
2. After that, ask the user for the arrival time and burst time of each process. Also input the time quantum.
3. In the loop, if time slot is greater than left burst time, execute process and find burst time.
4. Else if burst time is greater than time slot, execute it up to time slot and again push into the queue.
5. when the execution is completed, print the process information such as turnaround time and waiting time.

Time Complexity: O(total execution time)
All processes are executed up to their execution, so time complexity is O(total execution time).

Space Complexity: O(n)
Space is required to store burst time and arrival time, so space complexity is O(n).

Run Time Testcases
In this case, we enter “3” as the number of processes, and the arrival time and burst time are “p1: 0 10”, “p2: 1 8”, and “p3: 2 7” to find average waiting time and average turnaround time using Round Robin Scheduling algorithm. (Quantum Time = 5)

Enter Total Number of Processes:3
Enter Details of Process 1 
Arrival Time:  0
Burst Time:   10
Enter Details of Process 2 
Arrival Time:  1
Burst Time:   8
Enter Details of Process 3 
Arrival Time:  2
Burst Time:   7
Enter Time Slot:5
 
Process ID       Burst Time       Turnaround Time      Waiting Time
 
Process No 1  	     10		        20      	    10
Process No 2  	     8		        22		    14
Process No 3  	     7		        23		    16
 
Average Waiting Time: 13.333333
Avg Turnaround Time: 21.666666
