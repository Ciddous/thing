# How to Compile and Run Code
To compile the code you will either need to use a virtual machine or have gcc install into vscode. The easier and preffered method is a virtual machine, 
and the way will access this is by using your own dedicated server. If you don't have a server please contact your instructor to set one up for you. 
Will use PuTTY for our virtual machine, first we need to login using the instructions provied to you by your instructor.
Once logged in we need to add the processes.c file into the virtual machine, you'll using the following
pscp command with the syntax below

pscp [local_file_path] [username]@[hostname]:[remote_directory]

* [local_file_path] is the path of the processes.c file on your local machine
* [username] is your virtual machine username
* [hostname] is the IP Adress of your virtual machine
* [remote_directory] is the directory of your virtual machine of where you want to place the file

Next compile and run the file will first local which directory the file is and then access it. Then will 
use the following command to compile the file

gcc -o output_filename processes.c

* output_filename is the name of the output executable file

Then to run the file once it is compiled will use the command below

./output_filename
