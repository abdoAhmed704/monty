# Monty Bytecode Interpreter

## Table of Contents
- [Description](#description)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Opcodes](#opcodes)
- [Examples](#examples)
- [Authors](#authors)
- [License](#license)

## Description
The Monty Bytecode Interpreter is a program that processes Monty bytecodes, a scripting language that uses stacks and queues. The interpreter reads Monty bytecode files, executes the specified operations, and manages memory efficiently through the use of doubly linked lists.

## Technologies
- C programming language
- Data structures: Stack (LIFO) and Queue (FIFO)
- Memory management using dynamic allocation and deallocation

## Installation
To install and run the Monty Bytecode Interpreter, follow these steps:

1. Clone the repository:
   \`\`\`bash
   git clone https://github.com/abdoAhmed704/monty.git
   \`\`\`

2. Change directory into `monty`:
   \`\`\`bash
   cd monty
   \`\`\`

3. Compile the program:
   \`\`\`bash
   gcc -Wall -Werror -Wextra -pedantic *.c -o monty
   \`\`\`

## Usage
After compiling, the Monty interpreter can be run in the following modes:

- **Interactive Mode**: 
  Run the interpreter and type Monty bytecode instructions directly:
   \`\`\`bash
   ./monty
   \`\`\`

- **Non-Interactive Mode**: 
  Provide a Monty bytecode file as an argument to process the file's content:
   \`\`\`bash
   ./monty bytecode_file.m
   \`\`\`

## Features
- Processes Monty bytecode files that include stack and queue operations.
- Supports both stack (LIFO) and queue (FIFO) data structures.
- Efficient memory management using doubly linked lists.
- Error handling for edge cases and bytecode specifications.

## Opcodes
The Monty interpreter supports the following opcodes:
- `push`: Pushes an element onto the stack.
- `pall`: Prints all values in the stack/queue.
- `pop`: Removes the top element from the stack.
- `swap`: Swaps the top two elements.
- `add`: Adds the top two elements.
- Additional opcodes include `nop`, `sub`, `div`, `mul`, and more.

## Examples

1. Push two values and print all:
   \`\`\`bash
   $ echo "push 1\npush 2\npall" | ./monty
   2
   1
   \`\`\`

2. Execute a Monty bytecode file:
   \`\`\`bash
   $ cat file.m
   push 1
   push 2
   pall
   $ ./monty file.m
   2
   1
   \`\`\`

## Authors
- **Abdelrahman Ahmed Sayed** - [abdoAhmed704](https://github.com/abdoAhmed704)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
"""

# Write to a file
with open("/mnt/data/README_monty.md", "w") as file:
    file.write(monty_readme)
"/mnt/data/README_monty.md file created successfully!"

