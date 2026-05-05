# 1. Project Title: Unix Process Management and Executable Lifecycle Demonstration

## 2. Description
This project contains C source files and a custom Makefile demonstrating fundamental Operating Systems concepts, specifically focused on **Unix Process Management** (creation, backgrounding, control) and the **Executable Creation Pipeline** (the distinct roles of the Linker and the Loader).

The files implement demonstrations for:
* Process creation using fork().
* Process control using shell commands (sleep, ps, kill).
* The Linker's role in resolving external symbols across multiple files (file1jk.c and file2jk.c).
* The Loader's function in setting up memory and dynamic dependencies (ldd command).

## 3. Prerequisites & Installation
This project is intended for execution on a **Linux-based system** (such as Ubuntu/WSL).

### Prerequisites

* **GCC (GNU Compiler Collection):** Used for compiling and linking C source code.
* **make:** Used to automate the build and run process via the Makefile.
* **ldd:** The Linux utility for inspecting dynamic dependencies (usually pre-installed).

### Installation
To ensure you have the necessary tools on your Ubuntu Virtual Machine, run the following command:

sudo apt update
sudo apt install gcc build-essential

## 4. How to Build
The entire project is built using a single command defined in the Makefile. This process compiles all C files into their respective executable binaries.

make all
# or simply: make

*This command creates the executables: process_creation, role_of_linker, and role_of_the_loader.*

## 5. How to Run
Use the following make targets to execute the demonstrations for each exercise. Run these commands from the root directory of the assignment.

| Target | Action | Description |
| :--- | :--- | :--- |
| make run_ex1 | Process Creation | Executes the fork() demonstration. |
| make run_ex5 | Linker Role | Compiles and runs the demonstration showing two source files linked together. |
| make run_ex6 | Loader Role | Executes the program and runs ldd to list the dynamically loaded shared libraries. |
| make clean | Cleanup | Deletes all generated executable files. |

## 6. License
This project is licensed under the **MIT License**. See the separate LICENSE file for details.

## 7. Acknowledgments
This assignment was completed as part of the Operating Systems course (CSE233) at Alamein University.
