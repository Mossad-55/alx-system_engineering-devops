# Description for the scripts.
There is a simple rule to make a script we have to choose a specific line to define that the script will be executed using bash for example.
#### All scripts use the Shebang for bash shell:
* Execute the file using Bash shell (In this task we will use this one):
```
#!/bin/bash
```

## Tasks.

### 0. My name is Betty
* The script switches the current user to the a user called betty by using the ```su``` (Switch User)

### 1. Who am I

* The script prints the username of the current user.
* In this script we can use different commands:
    * ```id -u -n```
    * ```whoami```
    * ```echo $USER```

### 2. Groups

* The script prints all the goups that the current user is part of with the help of ```id -nG```

### 3. New owner 

* The script changes the owner of the file ```hello``` to the user ```betty``` by using ```sudo chown```

### 4. Empty! 

* The script create an empty file called ```hello``` in the current directory. Normal ```mkdir```

### 5. Execute 

* The scripts adds an execute permission to the owner of a file called ```hello``` by using ```chmod```

### 6. Multiple permissions 

* The script adds an execute permission to the owner and the group, and read permission to other users, to the file ```hello```. Used ```chmod``` as well

### 7. Everybody!

* The script adds execution permission to the owner, the group owner and the other users, to the file ```hello```
* I used the ```Symbolic mode``` because it wasn't allowed to write commas

### 8. James Bond

* The script sets the permission to the file ```hello``` as follows:
    * Owner: no permission at all
    * Group: no permission at all
    * Other users: all the permissions

### 9. John Doe 

* The script changes the file ```hello``` to this:
    * ```-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello```
* Not allowed to use comma so we will use ```chmod``` with Symbolic mode.

### 10. Look in the mirror 

* The script sets the mode of the file ```hello``` the same as ```olleh```'s mode by using ```chmod --reference```

### 11. Directories

* The script adds execute permission to all dubdirectories only. (No files at all). By using ```chmod -R ```

### 12. More directories

* The script creates a directory called ```my_dir``` with permissions 751 in the working directory by using ```mkdir -m```

### 13. Change group

* The script that changes the group owner to ```school``` for the file ```hello``` by using ```sudo chgrp```

### 14. Owner and group 

* The script changes the owner to ```vincent``` and the group owner to ```staff``` for all files and direcroties in the working directory by using ```chown -R newOwner:newGroup```

### 15. Symbolic links

* The same as previous script by we will add ```-h``` because it's a Symolic link and that will help us not change the reference of this link as well.

### 16. If only 

* The script changes the owner of the file ```hello``` to ```betty``` only if it's owned by ```guillaume``` by using ```chown --from=wanted_user```

### 17. Star Wars

* The script plays the StarWarsIV episode in the terminal by using ```telnet towel.blinkenlights.nl```
* Assuming that telnet was installed in the system.
