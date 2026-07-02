# Command Explanations - Question 2

- `umask`: I checked the current umask value to understand the default permissions assigned to newly created files and directories on the system.
- `mkdir -p project_workspace/docs project_workspace/code`: I used this to create a main project directory along with two subdirectories, using the `-p` flag to ensure parent directories are created if missing.
- `touch project_workspace/docs/design.txt`: I created an empty text file named design.txt to serve as a placeholder for testing file permissions.
- `ls -l project_workspace/docs/design.txt`: I ran this on the newly created file to observe its default permissions and ownership based on the system's umask.
- `chmod 700 project_workspace/code`: I changed the permissions of the code directory to 700 so that only the owner can read, write, and execute within it.
- `chown hritikshukla:staff project_workspace/docs/design.txt`: I explicitly set the user and group ownership of the file to ensure I maintain complete control over it.
