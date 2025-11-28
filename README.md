<div align="center"><img src="[https://github.com/vtiquet/holbertonschool-resources/blob/main/image/Holberton-Logo.svg](https://github.com/vtiquet/holbertonschool-resources/blob/main/image/Holberton-Logo.svg)" width=40% height=40%/></div>

## 🚀 Overview

This repository is a collection of solution files and projects completed as part of the **Holberton School** curriculum, focusing on **Shell, permissions, I/O redirection, and variable expansion** in Unix-like operating systems.

The tasks are organized into various directories, each representing a specific project or module.

## 📁 Directory Structure

| **Directory Name** | **Project/Module Topic** | **Description** | 
| :--- | :--- | :--- | 
| `basics` | **Shell Basics** | Introduction to fundamental shell commands like `pwd`, `ls`, `cd`, `mkdir`, `rm`, `mv`, and file manipulation. | 
| `permissions` | **File Permissions** | Scripts demonstrating how to view and modify file and directory permissions using `chmod`, `chown`, and `chgrp`. | 
| `init_files_variables_and_expansions` | **Init, Variables, and Expansions** | Tasks covering aliases, environment variables (`PATH`, `USER`), arithmetic operations, quoting, and shell expansions. | 
| `io_redirections_and_filters` | **I/O Redirections and Filters** | Scripts utilizing standard I/O redirection (`<`, `>`, `>>`, `|`), and filtering commands such as `head`, `tail`, `grep`, `sort`, `uniq`, and `tr`. | 

## 💡 Key Concepts Covered

### Shell Basics (`basics`)

* Current working directory (`pwd`)

* Listing files (`ls`, `ls -l`, `ls -a`)

* Changing directories (`cd`, `cd -`)

* Creating and deleting files/directories (`mkdir`, `rm`, `rmdir`)

* Copying and moving files (`cp`, `mv`)

* Creating symbolic links (`ln -s`)

### Permissions (`permissions`)

* Viewing user and group information (`whoami`, `groups`)

* Changing file ownership (`chown`)

* Changing file group (`chgrp`)

* Changing file permissions using octal and symbolic modes (`chmod`)

### Variables and Expansions (`init_files_variables_and_expansions`)

* Setting aliases (`alias`)

* Accessing environment variables (`$USER`, `$PATH`)

* Exporting variables (`export`)

* Arithmetic evaluation (`$(( ))`)

* Custom base conversions (binary to decimal, decimal to hexadecimal)

* String manipulation (`tr`, `rot13`)

### Redirection and Filtering (`io_redirections_and_filters`)

* Outputting text to files and stdout (`echo`, `cat`)

* Viewing file content (`head`, `tail`)

* Searching and counting lines/words (`grep`, `wc -l`)

* Filtering unique lines (`sort`, `uniq`)

* Finding files/directories (`find`)

* Reversing text (`rev`)

* Extracting fields (`cut`)

## 🛠️ How to Run the Scripts

All files in this repository are intended to be run as executable Shell scripts.

1. **Clone the repository:**

   ```bash
   git clone https://github.com/vtiquet/vtiquet-holbertonschool-shell.git
   cd vtiquet-holbertonschool-shell
````

2.  **Make a script executable:**
    Before running any file, ensure it has execute permission:

    ```bash
    chmod u+x basics/0-current_working_directory
    ```

3.  **Execute the script:**

    ```bash
    ./basics/0-current_working_directory
    ```

-----

## Authors

vtiquet - [GitHub Profile](https://github.com/vtiquet)