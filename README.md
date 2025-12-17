# get_next_line
A C project that implements a function to read a file descriptor line by line using a static buffer, handling memory management, EOF cases, and variable buffer sizes while respecting strict constraints and coding standards master

Features:
- Reads files and standard input line by line.
- Uses static storage to preserve state between calls.
- Works with any BUFFER_SIZE value.
- Handles EOF and errors safely.

Objectives:
- Understand and use static variables correctly.
-Manage dynamic memory safely without leaks.
-Read from files and standard input efficiently

Skills Learned:
- File I/O
- Static variables
- Memory management
- Defensive programming

Usage:
char *get_next_line(int fd);

Usage Example:
int fd = open("file.txt", O_RDONLY);
char *line;
while ((line = get_next_line(fd)))
{
    printf("%s", line);
    free(line);
}
