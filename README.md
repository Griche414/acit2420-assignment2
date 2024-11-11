# acit2420-assignment2

This assignment involves two small projects that involve using scripts to install packages along with their configurations, and another script to create a new user.

## Project 1: Configuration Scripts

This project consists of four files: the install-packages script, a plain-text file with a list of packages, the symbolic-links script, and the main config-script. The goal was to install packages and create symbolic links between configuration files stored in a remote repository and the user's home directory.

### install-packages Script
This script installs packages by reading a list of user-defined packages from the packages file. It stores the packages in an array and then uses a for loop to install each package.

### symbolic-links Script
This script creates symbolic links. It ensures that the user’s home directory is correctly set, using sudo, so that it doesn’t default to /root when running with elevated privileges.

### config-script Script
The main script, config-script, calls the install-packages and symbolic-links scripts when needed. It first checks if the script is run with sudo, then checks for any supplied options. If no options are given, it informs the user of the required flags. The script uses getopts to handle the options, which include installing packages, creating symbolic links, and cloning a remote repository.
