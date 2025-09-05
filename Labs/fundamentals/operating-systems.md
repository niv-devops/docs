# Operating Systems

The operating system (OS) is system software that manages the basic functionalities of a computer and is responsible for tasks such as process management, memory management, file system management, IO management, networking, security, and providing a user interface.

## Hardware Glossary

- **Binary Numbering System** - Built on a base of 2. Every time we reach a power of 2, we add another digit. The decimal system works the same way, just with 10.

- **Control Unit (CU)** – On a CPU receives information from the software; then, it distributes and directs the data to the relevant hardware components.

    !!! abstract "Some functions of the CU"
        - Determine what/where the next instruction must go for processing
        - Send clock signals to all hardware to force synchronous operations
        - Send memory taskings if appropriate

- **Arithmetic and Logic Unit (ALU)** - A digital circuit used to perform arithmetic and logic operations. It is the fundamental building block of the CPU.

    !!! abstract "Some ALU functions"
        - Addition & subtraction
        - Determining equality
        - AND/OR/XOR/NOR/NOT/NAND logic gates and more!

- **Registers** – A volatile memory system that provides the CPU with rapid access to information it is immediately using.

    !!! abstract "Functions of a register"
        - Store temporary data for immediate processing by the ALU
        - Hold "flag" information if an operation results in overflow or triggers other flags
        - Hold the location of the next instruction to be processed by the CPU

- **The CPU** - A Central Processing Unit (CPU) is the electronic circuitry that executes instructions based on an input of binary data (0’s and 1’s). The CPU consists of the `Control Unit (CU)`, the `Arithmetic and Logic Unit (ALU)`, and `registers (Immediate Access Store)`.


- **Random Access Memory (RAM)** - Additional high-speed memory that a computer uses to store and access information on a short-term basis.


- **Hard Disks / hard drives** - Responsible for the long-term, or secondary storage of data and programs.


- **The Mainboard / motherboard** - Printed circuit board that houses important hardware components via ports.


- **Ports** – A physical outlet used to connect devices to a computer. A computer typically contains multiple ports.


- **Main Functions of a Computer** - There are 4 main functions of a computer that make user interaction possible:

    1. **Input** - Data we give to our computers through interactions.
    2. **Processing** - Comprised of the translation of input and the instructions given for output.
    3. **Memory** - Used to store either temporary or permanent information.
    4. **Output** - The information that gets returned by the computer.


- **Throughput Measure** - Throughput is the total amount of data that can be transferred in a given amount of time.

    !!! abstract "Some common throughput numbers"
        - Smartphones: 500MB/Sec
        - Desktop drive: 5,000MB/Sec
        - RAM: 20,000MB/Sec

- **Latency Measure** - Latency is the amount of delay before that transfer of data begins.

    !!! abstract "Some common latency numbers"
        - Read from solid state drive: 150 microseconds
        - Ethernet connection: 10 milliseconds
        - 4G connection: 80 milliseconds
        - Satellite connection: 900 milliseconds

- **CPU and GPU Measures** - Both CPUs and GPUs have similar measures for computation performance. Each is made up of cores that can do one operation at a time, and these cores have set clock speeds that determine how often they can perform these operations.

- **Power Consumption Measure** - The energy devices use is measured in watts. The greater the wattage, the greater the amount of heat the device creates. Electricity costs can be a substantial part of the cost over the lifetime of the device.

## System Glossary

- **Bios (basic input/output system)** – A firmware used to provide runtime services for operating systems and programs and to perform hardware initialization during the booting process. It is a program the computer's microprocessor uses to start the computer system after it is powered on. It also manages data flow between the computer's operating system (OS) and attached devices, such as the hard disk, video adapter, keyboard, mouse and printer.

- **Boot Loader** - A computer program that is responsible for booting a computer. If it also provides an interactive menu with multiple boot choices then it's often called a boot manager.

- **RAM (Random-access memory)** – A form of electronic computer memory that can be read and changed in any order, typically used to store working data and machine code.

- **ROM (Read-only memory)** – A type of non-volatile memory used in computers and other electronic devices. Data stored in ROM cannot be electronically modified after the manufacture of the memory device. Read-only memory is useful for storing software that is rarely changed during the life of the system, also known as firmware.

- **CPU (central processing unit)** – A hardware component that's the core computational unit in a server. Servers and other smart devices convert data into digital signals and perform mathematical operations on them. The CPU is the primary component that processes the signals and makes computing possible. Its electronic circuitry executes instructions of a computer program, such as arithmetic, logic, controlling, and input/output (I/O) operations.

- **Binary / Octal / Hexadecimal**

    - **Decimal** represent any number using 10 digits [0–9].
    - **Binary** represent any number using 2 digits [0–1].
    - **Octal** represent any number using 8 digits [0–7].
    - **Hexadecimal** represent any number using 10 digits and 6 characters [0–9, A, B, C, D, E, F].

- **Kernel** - A computer program at the core of a computer's operating system and generally has complete control over everything in the system. The kernel is also responsible for preventing and mitigating conflicts between different processes. It is the portion of the operating system code that is always resident in memory and facilitates interactions between hardware and software components.

- **System Call** – A programmatic way in which a computer program requests a service from the kernel of the operating system it is executed on. A system call is a way for programs to interact with the operating system. This may include hardware-related services (for example, accessing a hard disk drive or accessing the device's camera), creation and execution of new processes, and communication with integral kernel services such as process scheduling. System calls provide an essential interface between a process and the operating system.

- **Bits .vs. Bytes**

    **A bit (Binary Digit)** is the smallest most basic unit of information in computing and digital communications. It's essentially a single binary data point, represents a logical state with one of two possible values. Either yes or no, on or off, up or down.
    
    **A byte** on the other hand is a unit of memory that usually contains 8 bits. This is because historically, 8 bits are needed to encode a single character of text. For this reason it is the smallest addressable unit of memory in many computer architectures.

## File System

The data structure used by the operating system to store and retrieve data.

- **Filesystem File** - A file is a unit of storage used to describe a self-contained piece of data and can have a variety of possible formats based on what that file contains.

- **Filesystem Directory** - A directory is a data structure that contains references to files and other directories. They are typically organized in a hierarchical tree structure called a directory tree.

- **Working Directory** - Also called a current directory, is the directory associated with the execution of a process.

- **File Attributes** - Collection of metadata that determine how files behave, such as if they are hidden or compressed.

- **File Permissions** - Determine which users and groups can read, write, and execute the file.

- **File Control Block** - Contains the metadata for a file, such as permissions and access times.

- **File and Directory Operations** - Both files and directories can be created, opened, read, written, deleted, closed, linked, unlinked, listed and truncated. It is possible to move across directories as well as find files within directories.

- **Filesystem Layers** - The filesystem has multiple layers of abstraction: The applications, logical file system, File-organization module, basic file system, IO control, and devices.

## Vim Editor

[Vim](https://www.vim.org), short for Vi IMproved, is a highly configurable text editor built to enable efficient text editing. It’s an enhanced version of the Vi editor, which was developed back in the 1970s.

!!! note "Built-in"
    Vim is a highly configurable text editor built to make creating and changing any kind of text very efficient. It is included as "vi" with most UNIX systems and with Apple OS X.

### Installation and Configuration

Most Linux distributions come with Vim pre-installed. However, if it’s not available on your system, you can install it using your package manager.

!!! info "Install Vim"
    === "Ubuntu/Debian"
        ```bash
        sudo apt-get install vim
        ```
    === "Arch Linux"
        ```bash
        sudo pacman -S vim
        ```
    === "macOS"
        ```bash
        brew install vim
        ```

### Modes in Vim

One of the unique features of Vim is its modes. Vim has several modes, each serving a different purpose:

- Normal Mode: This is the default mode when you first open Vim. In this mode, you can navigate the file,
delete text, copy text, and perform other commands.
- Insert Mode: Allows you to insert and edit text. To enter Insert Mode from Normal Mode, press `i`.
- Visual Mode: Here you can visually select blocks of text. To enter this mode from Normal Mode, press `v`.
- Command-Line Mode: This mode lets you enter Vim commands. To enter Command-Line Mode from Normal Mode, press `:`.


### Basic Commands in Vim

| Action                | Command/Keys                 |
|-----------------------|------------------------------|
| Saving a File         | `:w`                         |
| Exiting Vim           | `:q`                         |
| Force Quit            | `:q!`                        |
| Save and Quit         | `:wq`                        |
| Move Cursor           | `h`, `j`, `k`, `l` or arrows |
| Jump to Line Start    | `0`                          |
| Jump to Line End      | `$`                          |
| Jump to Specific Line | `:<line_number>`             |
| Delete Word           | `dw`                         |
| Delete N Words        | `d2w`                        |
| Delete Line           | `d$`                         |
| Undo                  | `u`                          |
| Redo                  | `Ctrl+r`                     |
| Search                | `/word`                      |
| Next Match            | `n`                          |
| Previous Match        | `N`                          |
| Replace Word          | `:s/searchword/replaceword/` |
| Replace All           | `:s/searchword/replaceword/g`|
| Replace with Confirm  | `:s/searchword/replaceword/gc`|
| Replace in Whole File | `:%s/searchword/replaceword/gc`|


### Text Editing

We have edited some text files before by using the i key. There are Four keys used for the insertion of text, Just type the key into the normal mode in vim:

| Key | Effect |
|-----|--------------------------------------------------|
| i   | Put cursor before the current position           |
| a   | Put cursor after the current position            |
| o   | Put cursor below the line                        |
| O   | Put cursor above the line                        |

Motion - Provide context to your Operators, These execute the action in a particular way:

| Motion | Effect                                             |
|--------|----------------------------------------------------|
| w      | Until the start of the next word (excluding first)  |
| e      | To the end of the current word (including last)     |
| $      | To the end of the line (including last character)   |

!!! tip "Motion"
    We can use motion with the `d` key and with many more keys.


!!! info "Count"
    The number for which replete the motion for count number. Here is a demonstration of the use of count and motion:

    - To move courser 2 words forward use the following command: `2w`.
    Here 2 is the number of counts and w is used for word.
    - To move the cursor 4 lines forward use the following command `4$`