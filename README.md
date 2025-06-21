# 📦 Huffman Compression & Decompression Tool

A complete file compression and decompression utility using the **Huffman Coding Algorithm** implemented in **C++**.

## 📂 Project Overview

This project implements the Huffman Coding algorithm to compress and decompress files efficiently, reducing storage size without losing any information (lossless compression). It includes:

- Huffman Tree construction using **priority queues**
- Generation of unique prefix codes for file characters
- Efficient **binary file storage** format with custom headers
- Complete decompression logic to restore original files


## 🛠️ Features

- **File Compression:** Converts input files into compressed `.huff` files.
- **File Decompression:** Restores compressed files to their original format.
- **Custom Data Structures:** Huffman Tree Nodes, Priority Queues.
- **Optimized File I/O:** Custom binary format with encoding metadata.



## 🚀 Technologies Used

- **C++ (STL, multithreading)**
- **Priority Queue (Min-Heap) for Huffman Tree**
- **Bit Manipulation for Binary Encoding**
- **File Streams (ifstream, ofstream)**

## ⚙️ How it Works

1. Frequency of each character in the file is counted.
2. A **Huffman Tree** is constructed where the path from root to leaf defines the **prefix code** for each character.
3. The file is encoded into a binary format and stored with a header containing the frequency table.
4. For decompression, the tree is reconstructed using the header to decode the file back to its original form.

