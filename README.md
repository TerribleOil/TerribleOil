# Ilia Laptiev

Software engineering student at NSTU in Novosibirsk, Russia. I write systems code in C and C++ and am moving toward distributed and data-intensive systems.

Most of my work is low-level: memory, processes, threads, and how they coordinate. I pay attention to how a program behaves under load and how its parts stay in sync, and that pulls me toward distributed systems.

## Current focus

**[parallel-radix-sort](https://github.com/TerribleOil/parallel-radix-sort)**: one sorting algorithm, four models of parallelism and inter-process communication.

I took a single algorithm, binary MSD radix sort (also called radix exchange sort), and implemented it four times, each over a different concurrency and IPC mechanism:

- Processes with POSIX shared memory (`mmap`), synchronized through `waitpid`
- POSIX threads with mutex-controlled parallelism
- Processes communicating over unnamed pipes
- Processes communicating over TCP sockets on localhost

I run the same benchmark on all four, on arrays up to 100 million integers, and compare performance across the coordination mechanisms.

## Next

A filesystem in C, from scratch: extent-based allocation, a B-tree of extents for file layout, an MFT-style index file, an LRU block cache, directory operations, a consistency checker, and an interactive shell.

## Stack

C, C++, POSIX, Linux (WSL). I use git, gdb, and standard command-line tooling.

## Contact

- Telegram: [@TerribleOil](https://t.me/TerribleOil)
- LinkedIn: [ilia-laptiev](https://www.linkedin.com/in/ilia-laptiev-8881bb421)
