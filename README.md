# 🗃️ Customised Virtual File System (CVFS) in C

A Customised Virtual File System developed in C that simulates essential file system operations using user-defined data structures. The system mimics real-world file operations such as create, read, write, open, close, delete, truncate, and seek.

---

## 🚀 Features

- Command-based file system interface
- In-memory simulation of file operations
- Supports:
  - `create` - Create new files
  - `open` - Open existing files
  - `write` - Write data to files
  - `read` - Read data from files
  - `close` - Close files
  - `ls` - List all files
  - `delete` - Delete files
  - `truncate` - Truncate file content
  - `lseek` - Move file pointer

---

## 🧱 Architecture

- **Superblock**: Stores total and free inodes
- **Inode Table (DILB)**: Stores metadata like file name, size, permissions
- **File Table**: Maintains file pointers, modes, and buffer positions
- **User File Descriptor Table (UFDT)**: Maps file descriptors to File Table entries

All components are implemented using **linked lists** and **dynamic memory allocation**.

---

## 🛠 Technologies Used

- **Language**: C
- **Concepts**:
  - File Handling
  - Data Structures (Linked Lists)
  - Memory Management

---

## ⚙️ How to Compile and Run

```bash
g++ cvfs.cpp -o cvfs
./cvfs
