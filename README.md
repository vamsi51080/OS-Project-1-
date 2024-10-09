# xv6 Commands Implementation: uniq and head

## Project Overview

This project involves the implementation of two essential Unix commands, `uniq` and `head`, in the xv6 operating system. Each command is developed both as a user program and as a kernel system call, providing a thorough understanding of operating systems and command-line utilities.

### Project Structure

The project is divided into two parts:

- **Part 1: Implementing `uniq` Command**
  - Task 1: User Space Implementation
  - Task 2: Kernel Space Implementation

- **Part 2: Implementing `head` Command**
  - Task 1: User Space Implementation
  - Task 2: Kernel Space Implementation

## Implementation Details

### Part 1: `uniq`

1. **User Space (`uniq.c`)**:
   - This program replicates the functionality of the `uniq` command, which filters out adjacent duplicate lines from an input file.
   - The user space program displays the message: *"Uniq command is getting executed in user mode,"* followed by the unique content.

   ```c
   // Example Output
   $ uniq OS611example.txt
   "Uniq command is getting executed in user mode."
   I understand the Operating system.
   I love to work on OS.
   Thanks xv6.
   ```

2. **Kernel Space**:
   - A system call named `uniq` is created that provides similar functionality, displaying the message: *"Uniq command is getting executed in kernel mode."*

### Part 2: `head`

1. **User Space (`head.c`)**:
   - This program replicates the functionality of the `head` command, which prints the first 14 lines of a specified file.
   - The user space program displays the message: *"Head command is getting executed in user mode,"* followed by the top lines of the input.

2. **Kernel Space**:
   - A system call named `head` is created that behaves similarly, displaying the message: *"Head command is getting executed in kernel mode."*

## Testing and Execution

- Ensure that the `Makefile` is set up correctly to compile both user and kernel programs.
- Use the following commands to test the implementations:
  ```bash
  make clean
  make qemu
  ```
- Verify the functionality by running the commands in the xv6 environment:
  ```bash
  uniq OS611example.txt
  head filename.txt
  ```


## Contribution

This project showcases my understanding of operating systems and Unix command implementation. 
## Contact Information

Feel free to reach out for collaboration or inquiries:

- **Name:** Vamsi Krishna Sripathi
- **Email:** vamsi51080@gmail.com
- **LinkedIn:** [[vamsi-sripathi](https://www.linkedin.com/in/vamsi-sripathi/)]
