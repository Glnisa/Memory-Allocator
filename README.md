[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/DNJSB_V7)

COMP 304 : Operating Systems
Project : Memory Allocator


kumalloc is a custom memory allocation function that aligns memory blocks and uses the sbrk system call to to get more data space. The function allocates and returns a block of memory with a size specified by the input parameter.

kucalloc function allocates memory for an array of elements, and initializes the memory content to zero.

kufree function deallocates the memory block pointed by the input pointer and adds it to the beginning of the free list. The function checks for a NULL pointer and returns early if there is a null pointer, avoiding unnecessary operations.

kurealloc function reallocates memory based on pointer and size. If the existing block is sufficiently large, it is resized in place; otherwise, a new block is allocated using kumalloc, data is copied from the old block, the old block is freed, and the new block is returned.

We also added helper methods for different operations such as splitting, merging, etc.

In total, we got 7.5 points. We couldn't implement the features that could pass the locality, fragmentation, unmap, and alternative design.

Implemented by Gülnisa Yıldırım 
