# Lab-8

This project simulates a Memory Management Unit (MMU) with memory allocation strategies: First Fit, Best Fit, and Worst Fit. The program processes an input file to allocate and deallocate memory for processes and perform coalescing of free memory blocks. The first line of the input file specifies the partition size, prefixed with -- (e.g., -- 100000). Subsequent lines represent operations such as allocation (<PID> <BlockSize>), deallocation (<-PID>), or coalescing (COALESCE). The program outputs the state of allocated and free memory after each operation.

To run the program, compile it using gcc -std=c99 -o mmu mmu.c list.c util.c -Wall -Werror and execute with ./mmu <input_file> <policy> where <policy> is -F (First Fit), -B (Best Fit), or -W (Worst Fit). Ensure the input file is correctly formatted, starting with a partition size line (e.g., -- 100000) followed by valid operations. Improperly formatted input will result in warnings or errors.
