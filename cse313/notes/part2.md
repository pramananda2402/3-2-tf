## Address spacce
- Memory Virtualization
- Precess Structure: struct thread
- user stack vs kernel stack
- benefit of memory virtualization
- multiprogramming and time sharing
- address space
- virtual space
- components of virtual space 

## Memory Api
- virtual address space
- malloc
- sizeof
- free
- memory allocating
- memory freeing
- forgetting to allocate memory
- not allocation enough memory
- forgotten to initialize
- memory leak
- Dangling pointer
- incorrect free
- calloc
- realloc
- sytemcall: nmap
- nmap: creating file-backed region
- nmap: creating anonymous region


## Address Translation
- memory virtualization with efficiency and control
- address translation
- Dynamic Relocation( Base and Bound Register)
- base and bound register
- dynamic(hardware based) relocation
- relocation and address translation
- two ways of bounds register
- hardware requirements
- os issue for memory virtualization
- os issue when process start running
- os issue when process terminate
- os issue when context switch
- os issue provide exception handelers

## Segmentation
- Inefficiency of Base and Bound Approach
- Segmentation
- placing segmentation in physical memory
- address translation on segmentation : code
- address translation on segmentation : heap
- segment fault or violation
- referring to segment
- segment selection
- fine grain and coarse grained segmentation
- os support: Fragmentation
- Memory compaction


## Free sapace management:
- manageing heap
- spliting
- coalescing
- tracking the size of allocated regions
- header of the allocated memory chunk
- embedding a free list
- heap initialization
- embedding a free list: allocation
- free space with chunk allocated
- free space with free
- free space with freed chunk
- double free
- growing the heap
- managing free spacea: basic strategies
- managing Free space: basic strategies
- segregated list: Mckusicks-kerels allocator
- Mckusicks-kerels allocator
- Buddy System
- Detailed Step
- Analysis
- Slab Allocator

## Paging
- concept of paging
- advantage of paging
- addresss translation
- where are the page table store
- Page table in kernel physical memory
- what is page table
- common flags of page table entry
- X86 page table  entry
- paging: too slow
- accessing memeory with paging
- a memory trace
- a virtual(and physical) memory trace


## Traslation Lookaside Buffer
- TLB 
- TLB basic algorithm
- Example: accessing an array
- locality
- whohandels the tlb miss
- TLB control flow algorithm(OS handled)
- TLB entry
- TLB issue: context switching
- To solve problem
- Another case 
- TLB replacement policy
- A real TLB entry 


## Advanced Page table
- Paging: Linear table
- Paging: smaller table
- problem
- hybride approach: Paging and Segments
- TLB miss in Hybride Approach
- problem of hybride approach
- Multi-level page table
- multi-level page table: Page directory
- multi-level page table
- Example
- single level page table Example
- two-level page table Example
- Page table index
- examples 
- more than two levels
- more than two level: page table index
- single level page table
- two level page table
- more than two level : page directory
- three level page table
- multi-level page table control flow
- the translation process: rememeber the TLB
- Inverted Page table


## Hard Disk Driver
- base geometry
- a simple disk Drive
- I/O time doing the math 
- Disk Scheduling: FCFS
- SSTF
- SCAN (elevator algorithm)
- C-SCAN
- C-LOOK
- select a disk schuduling algorithm
- disk schuduling


## RAID
- RAID (Redundant Array of Inexpensive Disks)
- Evalutation
- RAID Level 0
- RAID Level 1
- RAID Level 4
- RAID Level 5
- summery

## File and Directories
- concepts
- Interface: Creating a file
- Interface: Reading and Writting files
- abstraction 
- sample trace
- frok() and dup()
- fsync()
- renaming files
- getting information about files
- removing files
- making Directories
- reading Directories
- Deleting Directories
- Hard Links
- Unlink Hard Links
- Symbolic Links

## File System Implementation
- overview
- file system Implementation
- overall organization
- data region in file system
- inode table in file system
- allocation Structure
- super block
- file organization : the inode
- file structure : indexed allocation
- directory Structure
- file read 
- file Creation
- Caching and Buffering

 ## Crash Consistency : FSCK and Journaling

- overview
- a example of Crash Consistency
- crash senario
- solution
- Journaling
- Data Journaling
- Crash durinn Data Journaling
- To avoid data being inconsistent
- Recovery
- Batching Log update
- making the Log finite
- metadata Journaling
- Tricky case: block Reuse 
- Meta Data Jounaling Timeline
- data Journaling Timeline

## Log-Structure File System
- overview
- writting to disk sequentially
- segment
- Right  Segment size
- Finding inode
- The Check Point region
- Reading a file from the disk
- what about the Directories
- garbage
- garbage collection(Segment cleaning)
- Garbage collection
- segment summery block
- issue in garbage collection
- crash Recovery


## chapter -8 Multi -processor System
- Multiprocessor system
- UMA multiprocessor  with bus-based architecture
- UMA multiprocessor using crossbar Switches
- UMA multiprocessor using Multistage Switching Networks
- NUMA multiprocessor
- Each CPU has its own  OS
- master salve multiprocessor
- symmetric multiprocessor
- multiprocessor syschronization
- timesharing
- space sharing
- gang sharing


## cahpter-10: Linux
- History of Linux
- interface of linux
- kernal structure
- signals in linux
- process management system call in linux
- Memory managment in linux 
- memory managment system call in linux
- Physical memory management

## kernel memeory Allocator
- kernel memory allocator
- memory Fragmentation
- kernal allocator and virtual memory
- kernel allocation Characteristic
- Resource map Allocator
- Power of two Free List Allocators
- The Mckusicks-Karels Allocator
- Binary Buddy Allocator