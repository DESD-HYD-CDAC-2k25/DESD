## OS MODULE EXAM
Ques OS BATCH 1

I. Implement the following requirements using Operating system ( Use UNNamed PIPES )

- System has two processes P1 and p2 
- p1 opens a file <any file>
- p1 reads 256 bytes of data from the file and sends it to P2
- P2 counts the occurence of the letter 'A' and 'Z' in the incoming data from P1
- P2 prints the number of Occurences of 'A' and 'Z' letters.

II. Implement the following requirements using Operating system ( use Message Queue )

- System has two processes P1 and p2 
- P1 opens a file < any file>
- p1 reads 256 bytes of data from the file and sends it to P2
- P2 counts the occurence of the letter 'A' and 'Z' in the incoming data from P1
- P2 prints the number of Occurences of 'A' and 'Z' letters.



Ques OS BATCH 2

I. Implement the following requirements using Operating system ( Use Shared Memory )

- System has two processes P1 and p2 
- p1 opens a file <any file>
- p1 reads 256 bytes of data from the file and sends it to P2
- P2 counts the occurence of the letter 'A' and 'Z' in the incoming data from P1
- P2 prints the number of Occurences of 'A' and 'Z' letters.

II. Implement the following requirements using Operating system ( use Message Queue )

- System has two processes P1 and p2 
- P1 opens a file < any file>
- p1 reads 256 bytes of data from the file and sends it to P2
- P2 counts the occurence of the letter 'A' and 'Z' in the incoming data from P1
- P2 prints the number of Occurences of 'A' and 'Z' letters.

## LDD

Q1) Basic character Driver Development

A. Write a basic character driver that implements driver that implements:
 open(), read(), write(), close().
Print messages in each function to indicate when they are called.

B. Modify the basic driver to support a fixed-size kernel buffer(e.g.100 bytes)
    store return data in the buffer.
    Read return the data from the buffer.
C. Implement an IOCTL command to clear the kernel buffer.

D. Verify User Read/Write operations using IOCTL functionality.


Q2) Kernel synchronization mechanism for multiple devices.

A. Write a character for Multiple devices and create 2 devicenumbers. 
Use spinlock to protect the Critical section ( write activity ) and 
    Use wait queues to avoid consecutive write operations.

B. Put the write function to sleep using wait-queues after successful write operation before releasing spinlock.
C. Wake-up sleep (wait-queues) operation only in read function.
D. Maintain a Kernel buffer of 50 bytes to read and Write data.
E. Write 2 seperate programs for Read and Write for each device.


Q3) GPIO and LED

A. Write a basic GPIO driver to turn an LED ON/OFF using IOCTL.
B. Use a kernel timer to blink the LED every 1 second.
C. Add an IOCTL to change the blink interval dynamically.

##RTOS

BATCH-2

Q1. Implement a RTOS application where a periodic software timer sends integer data to a task via a Message Buffer.

Your task is to implement the following:

TASKS 1 priority 8

TASKS 2 priority 6

Task 1:

- This task continuously receives integer data from the message buffer every 3 seconds.

Task 2:

- This task creates and starts a periodic software timer that triggers every 1 second and task2 deletes itself after starting the timer.

- The timer callback should generate an integer value and send it to a message buffer.

- The integer value should start at 0 and be incremented with each timer callback.

Q2. Implement a RTOS application that demonstrates inter-task communication of integer data using message queues. The application should involve 4 tasks, 2 tasks sending the data through message queue every 2 seconds and 2 tasks receiving data through message queue every 5 seconds.

periodicity and priorities of the tasks are as follows

TASKS 1 priority 8

TASKS 2 = priority 6

TASKS 3 priority 4

TASKS 4 priority 2


‎Task1‎<--|‎ ‎ ‎‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎             |--<-Task3
‎ ‎ ‎ ‎ ‎ ‎ ‎‎  ‎ ‎ ‎ ‎ ‎   | --‎ MQUEUE<----|
Task2 ‎<-| ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎          |--<-Task4