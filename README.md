# Low-Level C/C++ Projects

This repository is a personal playground for exploring low-level programming concepts with C and C++. The goal is to build small, focused projects that improve understanding of systems programming, memory management, pointers, file I/O, process control, networking, and other close-to-the-metal topics.

## Purpose

This workspace is meant for:

- learning C and C++ in a practical way
- building small low-level utilities and experiments
- understanding memory, CPU, and OS-level behavior
- practicing debugging, profiling, and optimization
- collecting reusable patterns for future systems projects

## Project Style

Each project is intended to be:

- small and self-contained
- written in C or C++ where appropriate
- focused on a specific concept or system feature
- easy to compile and test locally
- suitable for experimentation and learning

## Recommended Layout

A simple structure for future projects could look like this:

```text
low-level/
├── README.md
├── .gitignore
├── project-name/
│   ├── src/
│   ├── include/
│   ├── tests/
│   ├── Makefile
│   └── README.md
├── cat/
│   ├── cat.c
│   └── cat.exe
├── notes/
│   └── ideas.md
└── build/
```

## Tooling

Common tools used in this kind of work:

- GCC / Clang
- G++ for C++ projects
- Make or CMake
- GDB for debugging
- Valgrind for memory checking
- ASan / UBSan for sanitizer-based debugging
- Shell tools for testing and automation

## Getting Started

### Compile a C program

```bash
gcc -Wall -Wextra -std=c11 -o program src/program.c
./program
```

### Compile a C++ program

```bash
g++ -std=c++17 -Wall -Wextra -O2 -o program src/main.cpp
./program
```

### Build a project with Make

```bash
make
./program
```

## Example Project

The `cat/` directory currently contains a small C-based utility experiment. It is a simple example of working with file input, loops, and low-level I/O patterns.

## Learning Focus

Possible future projects in this repo may include:

- custom `ls` implementation
- minimal `cp` or `cat` tools
- memory allocator experiments
- linked list and tree data structures
- thread and mutex examples
- socket programming
- file system utilities
- ELF or binary parsing experiments
- compiler/interpreter toy projects

## Best Practices

- compile with warnings enabled
- check for memory leaks and invalid access
- keep programs small and readable
- test edge cases and boundary conditions
- prefer explicit behavior over hidden magic
- document assumptions and design choices

## Notes

This repository is intentionally practical and experimental. The idea is to build things hands-on and learn by implementing small systems-level programs rather than only reading theory.

## Next Step

Create a new folder for each project, write the code, compile it locally, and keep notes on what was learned. Over time, this repo will become a collection of system-level programming experiments and reusable low-level implementations.
