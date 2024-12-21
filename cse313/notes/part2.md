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

