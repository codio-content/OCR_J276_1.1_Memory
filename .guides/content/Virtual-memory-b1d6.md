When the CPU is running several programs at the same time (multitasking) the RAM can become full. 
Instead of closing some programs, the operating system will use an area of a storage device, usually the hard disk drive, to store some of the instructions and data.
This area is called ‘virtual memory’ because it is simulating the RAM.

Operating systems such as Windows allow you to change the size of hard disk drive reserved for virtual memory. It is called a paging file.
![](.guides/img/paging.png)

If there is no free memory, the memory manager will ‘swap out’ some of the data stored in RAM to the swap area (virtual memory) on the hard disk drive and load the requested data into the now free area.
Usually the least recently used stored data is swapped out.

If data is swapped out and then is needed again, it is swapped back in, from the swap area, at the expense of other data.

There are disadvantages of using virtual memory:

- The read/write speed of a hard drive is much slower than RAM, and the technology of a hard drive is not geared towards accessing small pieces of data at a time.
- If the system has to rely too heavily on virtual memory, there will be a significant performance drop.

Often the operating system has to constantly swap information back and forth between RAM and the hard disk drive, which has to operate all of the time.
This is called ‘disk thrashing’ and significantly slows down the execution of the programs.