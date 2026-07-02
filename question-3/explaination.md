# Command Explanations - Question 3

- `touch original_file.txt` & `echo "Hello Linux" > original_file.txt`: I created a new file and used the redirection operator to write a string of text into it for testing links.
- `ln original_file.txt hard_link.txt`: I created a hard link to the original file, generating a new directory entry that points to the exact same inode.
- `ln -s original_file.txt sym_link.txt`: I created a symbolic (soft) link, which creates a separate file with a distinct inode that simply points to the original file's path.
- `ls -li original_file.txt hard_link.txt sym_link.txt`: I displayed the files alongside their inode numbers to observe that the original and hard link share an inode, while the soft link does not.
- `rm original_file.txt`: I deleted the original file to observe how the deletion of the source affects both the hard link and the symbolic link.
- `cat hard_link.txt` & `cat sym_link.txt`: I attempted to read both links, observing that the hard link retained the data while the symbolic link returned a "No such file or directory" error.
