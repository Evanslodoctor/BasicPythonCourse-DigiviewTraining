# Lesson: File Operations

## Introduction

In this lesson, we'll explore essential file operations in Linux, including copying, moving, renaming, and deleting files and directories. Understanding these operations is fundamental for effective file management on a Linux system.

## Working with Files and Directories

### `cp` - Copy Files and Directories

- Syntax: `cp [options] source destination`
- Examples:
  - `cp file1.txt file2.txt`: Copy file1.txt to file2.txt.
  - `cp -r directory1 directory2`: Recursively copy directory1 and its contents to directory2.

### `mv` - Move (Rename) Files and Directories

- Syntax: `mv [options] source destination`
- Examples:
  - `mv file1.txt newfile.txt`: Rename file1.txt to newfile.txt.
  - `mv file1.txt directory/`: Move file1.txt to the directory.

### `rm` - Remove (Delete) Files and Directories

- Syntax: `rm [options] file`
- Examples:
  - `rm file1.txt`: Remove file1.txt.
  - `rm -r directory`: Recursively remove the directory and its contents.

### `rmdir` - Remove (Delete) Directories

- Syntax: `rmdir [options] directory`
- Examples:
  - `rmdir directory`: Remove the directory if it's empty.
  - `rmdir -p parent/child`: Remove parent and child directories recursively.

## Viewing File Contents

### `cat` - Concatenate and Display File Contents

- Syntax: `cat [options] file`
- Examples:
  - `cat file1.txt`: Display the contents of file1.txt.
  - `cat file1.txt file2.txt`: Concatenate and display the contents of file1.txt and file2.txt.

### `less` - View File Contents Page by Page

- Syntax: `less [options] file`
- Examples:
  - `less file1.txt`: View the contents of file1.txt page by page.
  - `less +F file1.txt`: View file1.txt and keep checking for updates.

### `head` and `tail` - View the Beginning and End of Files

- Syntax: 
  - `head [options] file`: Display the first part of a file.
  - `tail [options] file`: Display the last part of a file.
- Examples:
  - `head file1.txt`: Display the first 10 lines of file1.txt.
  - `tail -n 20 file1.txt`: Display the last 20 lines of file1.txt.

## Searching Through Files

### `grep` - Search Text Patterns in Files

- Syntax: `grep [options] pattern [file(s)]`
- Examples:
  - `grep "keyword" file1.txt`: Search for the keyword in file1.txt.
  - `grep -r "pattern" directory/`: Recursively search for the pattern in the directory.

## Conclusion

This lesson covers essential file operations in Linux, empowering you to efficiently manage files and directories from the command line. Each operation is accompanied by syntax explanations and practical examples for better comprehension.
