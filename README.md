# Huffman Compression and Decompression

## Overview

This repository contains a command-line utility for data compression and decompression using Huffman coding. The project involves debugging, optimizing, and improving an existing implementation of the program `huff`.

## Program Features

The huff program performs two primary operations:

-**Compression**: Encodes input data using Huffman coding, producing a compressed output.

-**Decompression**: Decodes compressed data to recover the original input.

## Usage
The program supports the following command-line arguments:

`bin/huff [-h] [-c|-d] [-b BLOCKSIZE]`
-    -h       Help: displays this help menu
-    -c       Compress: read raw data, output compressed data
-    -d       Decompress: read compressed data, output raw data
-    -b       For compression, specify blocksize in bytes (range [1024, 65536])

## Tools and Techniques

### Debugging Tools:

- gdb for step-by-step debugging.

- valgrind to detect memory leaks and invalid memory accesses.

### Profiling Tools:

- gprof to analyze program performance and identify optimization opportunities.

### Example Usage

- **Compression**

`bin/huff -c -b 4096 < input.txt > compressed.huff`

- **Decompression**

`bin/huff -d < compressed.huff > output.txt`

- **Display Help**

`bin/huff -h`

