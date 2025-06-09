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

##LDD

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
A. Write a character for Multiple devices and create 2 devicenumbers. Use spinlock to protect theCritical section ( write activity ) and 
    Use wait queues to avoid consecutive write operations.

B. Put the write function to sleep using wait-queues after successful write operation before releasing spinlock.
C. Wake-up sleep (wait-queues) operation only in read function.
D. Maintain a Kernel buffer of 50 bytes to read and Write data.
E. Write 2 seperate programs for Read and Write for each device.

Q3) GPIO and LED

A. Write a basic GPIO driver to turn an LED ON?OFF using IOCTL
B. Use a kernel timer to blink the LED every 1 second.
C. Add an IOCTL to change the blink interval dynamically.