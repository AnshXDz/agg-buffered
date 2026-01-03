# agg-buffered

Problem: Copying a huge number of small files is slow due to filesystem overhead.

Goal: Reduce copy time without compression by minimizing filesystem operations.

Approach: Bundle many small files into a single container file and restore them later(Using File aggregation and buffering I/O).
