# acit2420-assignment2

This assignment involves two small projects that involve using scripts to install packages along with their configurations, and another script to create a new user.

## Project 1: Configuration Scripts

This project includes four files: the install-packages script, a list of packages text file, the create-symlinks script, and the config-setup script. 

### install-packages Script
This script installs packages by reading a list of packages from the packages file.

### create-symlinks Script
This script creates symbolic links. 

### config-setup Script
This script calls upon the other 2 scripts when needed to install the packages, create symbolic links, and cloning a remote repository.

Run the config-setup.sh with sudo and supply it with -c, -i, -s

# Project 2: New User Script
This project contains a script that can add new users with a shell and password, then add them to groups.

usage for the script is given as ```sudo ./new-user-script -u <username> -s <shell> -g <group1,group2,...>``` 
be sure to supply the <> fields with the actual names

