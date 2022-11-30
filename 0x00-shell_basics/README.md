# Description for the scripts.
There is a simple rule to make a script we have to choose a specific line to define that the script will be executed using bash for example.
#### Examples for typically Shebang lines:
* Execute the file using Bourne shell:
```
#!/bin/sh
```
* Execute the file using Bash shell (In this task we will use this one):
```
#!/bin/bash
```
* Execute the file using PowerShell:
```
#!/usr/bin/pwsh
```
* Execute the file using a Python interpreter:
```
#!/usr/bin/env python3
```

### 0. Where am i?

* The script should print the current working directory
* We will use the Shebang file for bash shell and the second line we will put the command for printing the current directory. 
```
#!/bin/bash
pwd
```

### 1. What’s in there?

* Our script should list all the directories and files in the current directory. 
```
#!/bin/bash
ls
```

### 2. There is no place like home

* Script for changing the current directory to the user's home directory.
```
#!/bin/bash
cd ~ or cd 
```

### 3. The long format

* Display current directory contents in a long format 
```
#!/bin/bash
ls -l
```

### 4. Hidden files

* Display current directory contents in a long format as well as the hiddent ones. 
```
#!/bin/bash
ls -al
```

### 5. I love numbers

* Display directory contents in :
    * Long format
    * with user and group IDs displayed numerically
    * And hidden files (starting with .)
```
#!/bin/bash
ls -aln
```

### 6. Welcome

* Script that creates a directory named my_first_directory in /tmp/ directory
```
#!/bin/bash
mkdir /tmp/my_first_directory/
```

### 7. Betty in my first directory

* Script that moves the file betty from /tmp/ to /tmp/my_first_directory.
```
#!/bin/bash
mv /tmp/betty /tmp/my_first_directory/
```

### 8. Bye bye Betty

* Delte the file betty that we created before. 
```
#!/bin/bash
rm /tmp/my_first_directory/betty
```

### 9. Bye bye My first directory

* Delete the directory my_first_directory that is in the /tmp directory.
```

#!/bin/bash
rmdir /tmp/my_first_directory 
# We can use the rm -r 
```

### 10. Back to the future

* Takes the user to the previous working directory
```
#!/bin/bash
cd -
```

### 11. Lists

* A script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format
```
#!/bin/bash
ls -al . .. /boot
```

### 12. File type

* Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.
```
#!/bin/bash
file /tmp/iamafile
```

### 13. We are symbols, and inhabit symbols

* Script for creating a symbolic link to /bin/ls named __ls__ in the current directory.
```
#!/bin/bash
ln -s /bin/ls __ls__
```

### 14. Copy HTML files

* Script for copying all the HTML files to the parent of the current directory.
```
#!/bin/bash
cp -u *.html ..
```

### 15. Let’s move

* Script that moves all files beginning with an uppercase letter to the directory /tmp/u.
```
#!/bin/bash
mv [[:upper:]]* /tmp/u 
```

### 16. Clean Emacs

* A script to delete all files that end with ~.
```
#!/bin/bash
rm -r *~
```

### 17. Tree

* a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.
    * Note: Only two spaces allowed.
```
#!/bin/bash
mkdir -p welcome/to/school
```

### 18. Life is a series of commas, not periods

* A script to list all the content of the current directory, separated by commas and directory name should end with /
```
#!/bin/bash
ls -apm
```

### 19. File type: School

* a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0.
```
0 string SCHOOL School data
!:mime School
```

# Notes
* Before we use ``` git add . ``` with the bash scripts we have to convert the file into executable file by using the following command:
    ```
    chmod u+x file_name
    ```
* Before ``` git add . ``` in the magic file task use the following command:
    ```
    file -C -m school.mgc
    ```

## You are all set :) Don't forget to star this repo. 
