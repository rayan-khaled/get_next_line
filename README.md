# get_next_line

**Summary**

The goal of this project is to implement a function that reads a file descriptor line by line.
It introduces the use of static variables and focuses on efficient memory management and file I/O in C, maste

**Features:**

- Reads files and standard input line by line.
- Uses static storage to preserve state between calls.
- Works with any BUFFER_SIZE value.
- Handles EOF and errors safely.

**Objectives:**

- Understand and use static variables correctly.
-Manage dynamic memory safely without leaks.
-Read from files and standard input efficiently

**Skills Learned:**

- File I/O
- Static variables
- Memory management
- Defensive programming

**Usage:**

char *get_next_line(int fd);

**Usage Example:**
int fd = open("file.txt", O_RDONLY);
char *line;
while ((line = get_next_line(fd)))
{
    printf("%s", line);
    free(line);
}

**Author:**

Rayan Khaled
[rayan-khaled]
[rayannkhaled@outlook.com]
