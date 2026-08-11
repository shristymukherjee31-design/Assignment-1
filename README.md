# Assignment-1.2
Linux File & Directory Management Utility

Overview

This project contains a Bash script named FileManager.sh that automates common Linux file and directory operations. The script accepts command-line arguments to perform operations such as creating directories, managing files, displaying file content, copying, moving, and deleting files.



Project Structure

```text
Assignment1/
├── FileManager.sh
├── README.md
└── images/
    ├── setup.png
    ├── directory-operations.png
    ├── file-content.png
    ├── beginning-content.png
    ├── read-operations.png
    ├── move-copy.png
    └── delete-operations.png
```



Getting Started

Give execute permission to the script.

```bash
chmod +x FileManager.sh
```

Run the script using:

```bash
./FileManager.sh <operation> <arguments>
```

Example:

```bash
./FileManager.sh addDir /tmp dir1
```



Directory Operations

Supported operations:

• Create Directory

• Delete Directory

• List Files

• List Directories

• List All Contents

Example:

```bash
./FileManager.sh addDir /tmp/test dir1
./FileManager.sh addDir /tmp/test dir2
./FileManager.sh addDir /tmp/test dir3

./FileManager.sh listFiles /tmp/test
./FileManager.sh listDirs /tmp/test
./FileManager.sh listAll /tmp/test

./FileManager.sh deleteDir /tmp/test dir3
```

Output

![Directory Operations](images/directory-operations.png)



File Creation and Content Operations

Supported operations:

• Create File

• Create File with Initial Content

• Append Content to File

• Add Content at the Beginning of File

Example:

```bash
./FileManager.sh addFile /tmp/dir1 file1.txt

./FileManager.sh addContentToFile /tmp/dir1 file1.txt "Hello Linux"

./FileManager.sh addContentToFile /tmp/dir1 file1.txt "Learning Bash"

./FileManager.sh addContentToFileBegining /tmp/dir1 file1.txt "First Line"
```

Output

![File Operations](images/file-content.png)

Beginning Content

![Beginning Content](images/beginning-content.png)



Reading File Content

Supported operations:

• Show First N Lines

• Show Last N Lines

• Show Content at Specific Line

• Show Content for Line Range

Example:

```bash
./FileManager.sh showFileBeginingContent /tmp/dir1 file1.txt 3

./FileManager.sh showFileEndContent /tmp/dir1 file1.txt 2

./FileManager.sh showFileContentAtLine /tmp/dir1 file1.txt 2

./FileManager.sh showFileContentForLineRange /tmp/dir1 file1.txt 2 4
```

Output

![Read Operations](images/read-operations.png)



Move and Copy Operations

Example:

```bash
./FileManager.sh moveFile /tmp/dir1/file1.txt /tmp/dir2/

./FileManager.sh copyFile /tmp/dir2/file1.txt /tmp/dir1/
```

Output

![Move and Copy](images/move-copy.png)



Clear and Delete Operations

Example:

```bash
./FileManager.sh clearFileContent /tmp/dir1 file1.txt

./FileManager.sh deleteFile /tmp/dir1 file1.txt

./FileManager.sh deleteDir /tmp dir3
```

Output

![Delete Operations](images/delete-operations.png)



Project Setup

The script requires execute permission before running.

```bash
chmod +x FileManager.sh
```

Output

![Project Setup](images/setup.png)



Linux Commands Used

• mkdir

• rmdir

• rm

• ls

• grep

• touch

• echo

• cat

• head

• tail

• mv

• cp



Learning Outcome

Through this assignment, I learned:

• Bash scripting using case statements

• Working with command-line arguments

• File and directory management in Linux

• Reading file content using head and tail

• Copying and moving files

• Clearing and deleting files

• Using basic Linux commands in shell scripting



Author

Shristy Mukherjee
