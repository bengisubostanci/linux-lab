Linux File and Directory Management Guide
This guide covers essential Linux terminal commands for creating, listing, and removing files and directories, including advanced filtering techniques.

1. Creating Files and Directories
Create a File (touch)
The touch command is primarily used to create empty files or update timestamps.

touch my_file

ls -l
# total 0
# -rw-rw-r--. 1 user user 0 Sep  1 16:41 my_file

Create a Directory (mkdir)
To create a new directory, use mkdir. You can also use the -p flag to create parent directories simultaneously if they don't exist.

mkdir myfolder
mkdir -p nested/folder/structure

2. Removing Files and Directories (rm)

The rm command removes data. By default, it does not delete directories unless specific flags are used.

Flag,Description
-f,"Force: Ignore nonexistent files and arguments, never prompt."
"-r, -R",Recursive: Remove directories and their contents recursively.
-i,Interactive: Prompt before every removal.
-v,Verbose: Explain what is being done.

Removing a File
rm my_file

Removing a Directory
Standard rm will fail on directories:
rm myfolder/
# rm: cannot remove 'myfolder/': Is a directory

To successfully delete a directory and its contents, use the recursive flag:
rm -r myfolder

3. Advanced: Removing All Files Excluding Specific Ones
To delete everything in a directory except for one or more specific files, you can utilize Bash extended globbing.

Step 1: Enable Extended Pattern Matching
This feature might be disabled by default in your shell. Enable it using shopt:
shopt -s extglob

Step 2: Delete with Exclusion
⚠️ Warning: Always double-check your target directory before running destructive commands.

Exclude a single file:
rm -vr !("configmap.yaml")

Exclude multiple files or folders:
Use the pipe (|) character as an OR operator inside the parenthesis.

rm -vr !("configmap.yaml"|"deployment.yaml"|"tests")

Practical Example
Initial State:
ls -l
# total 32
# -rw-rw-r-- 1 user user  117 Aug 24 11:00 configmap.yaml
# -rw-r--r-- 1 user user 1836 Aug 24 11:00 deployment.yaml
# -rw-r--r-- 1 user user  916 Aug 24 11:00 hpa.yaml
# -rw-r--r-- 1 user user 1056 Aug 24 11:00 ingress.yaml
# drwxr-xr-x 2 user user   34 Aug 24 11:00 tests

Execution
rm -vr !("configmap.yaml")
# removed ‘deployment.yaml’
# removed ‘hpa.yaml’
# removed ‘ingress.yaml’
# removed ‘tests/test-connection.yaml’
# removed directory: ‘tests’

Final Result:
ls -l
# total 4
# -rw-rw-r-- 1 user user 117 Aug 24 11:00 configmap.yaml

Quick Tip
If you want to safely test what would be deleted before actually deleting it, replace rm -vr with ls -d:
ls -d !("configmap.yaml")



