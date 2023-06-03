- Our kernel has to manage our resources efficiently so that all the programs we want to use can be run. Our kernel doesn't just dedicate all of our computers resources to one process. Our system is actually constantly running multiple processes that are necessary for it to function. Our kernel has to worry about all of these processes at once.

- The kernel has to schedule time for the CPU to execute the instructions in the process, but there's only one CPU and many processes.

- The cpu executes processes one-by-one through something known as a time slice. A time slice is a very short interval of time that gets allocated to a process for CPU execution.

#kernel #process-management #course1-module3 