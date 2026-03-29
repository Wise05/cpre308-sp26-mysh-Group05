Group 5

Stage 1 - Completed by Ambrose Schnaufer
Stage 2 - Completed by Lukas Hessling
Stage 3 - Completed by Zevan Gustafson
Stage 4 - Completed by Shane Nebraska

Known Limitations: Some known limitations include only one pipe at a time being supported, no background processes, and no signal handling.

Pipe Description: At the start of this stage a pipe is created with both a read and write end. Next two child processes are forked. The left child is the writer while the right child is the reader. Each child redirects the output/input to/from the pipe and closses unused pipe ends. Afterwards they execute their corresponding command with execvp. The parent process closes both ends of the pipe and waits for both of the children processes to complete.
