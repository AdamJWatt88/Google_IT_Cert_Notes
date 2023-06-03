-   Use `top` command to see real-time **system utilization** and **top processes** that are using resources. To get out of top use the `q` command
-   Check **"percentage CPU"** and **"percentage MEM"** fields to see CPU and memory usage of a single task.
-   Use `uptime` command to see current time, system uptime, number of logged-in users, and load average of machine.
-   **Load averages** show average CPU load in one, 5, and 15 minute intervals, and are useful to see how a machine is doing over a period of time.
-   Use `lsof` command to **list open files** and what processes are using them.
-   Monitor hardware utilization separately from processes using various commands.
-   If **managing a fleet of machines**, consider **monitoring hardware utilization** for all machines at once.
-   Understanding how to read process information and manage processes is vital for troubleshooting issues as an IT support specialist.

# Supplemental reading for Resource Monitoring in Linux

# Resource Monitoring in Linux

Balancing resources keeps a computer system running smoothly. When processes are using too many resources, operating problems may occur. To avoid problems from the overuse of resources, you should monitor the usage of resources. Monitoring resources and adjusting the balance is important to keep computers running at their best. This reading will cover how to monitor resources in Linux using the load average metric and the common command.

# Load in Linux

In Linux, a load is the set of processes that a central processing unit (CPU) is currently running or waiting to run. A load for a system that is idle with no processes running or waiting to run is classified as a 0. Every process running or waiting to run adds a value of 1 to the load. This means if you have 3 applications running and 2 on the waitlist, the load is 5. The higher the load, the more resources are being used, and the more the load should be monitored to keep the system running smoothly. 

# Load average in Linux

The load as a measurement doesn’t provide much information as it constantly changes as processes run. To account for this, an average is used to measure the load on the system. The load average is calculated by finding the load over a given period of time. Linux uses three decimal values to show the load over time instead of the percent other systems use. An easy way to check the load average is to run the uptime command in the terminal. The following image depicts the load values returned from the uptime command. 

![Load average values returned in the Linux terminal](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/pgFymc0qRieBcpnNKuYnhA_cd15354ef56145d98a3e1692be115ef1___Load-Average.png?expiry=1683331200000&hmac=4yBxclDNduxFCQlRyWBgZWjGiV6l9sZJrHcOYDRjX7s)

The command returns three load averages:

1.  **Average CPU load for last minute,** which corresponds to 0.03. This is a very low value and means an average of 3% of the CPU was used over the last minute. 
    
2.  **Average CPU load for last 5 minutes** corresponds to the second value of 0.03. Again, this can be thought of as, on average, 3% of the CPU was being used over the past five minutes. 
    
3.  **Average CPU load for last 15 minutes** corresponds to 0.01, meaning on average, 1% of the CPU has been used over the last 15 minutes. 
    

# Top

Another way you can monitor the load average in Linux is to use the top (table of processes) command in the terminal. The result of running the top command is an in-depth view of the resources being used on your system. 

![Detailed process load average output in Linux terminal](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/5Kn9dki-TDSp_XZIvqw0Sw_68859d29f8d74a80811f44d1820f58f1___Top.png?expiry=1683331200000&hmac=LRhVrI62hSLghGu7kLBOyZ_Nt64CxAE_5UdCeedVpFo)

The first line displayed is the same as the load average output given using the uptime command It lists what percent of the CPU is running processes or has processes waiting. The second line shows the task output and describes the status of processes in the system. The five states in the task output represent:

1.  **Total** shows the sum of the processes from any state. 
    
2.  **Running** shows the number of processes currently handling requests, executing normally, and having CPU access.
    
3.  **Sleeping** shows the number of processes awaiting resources in their normal state. 
    
4.  **Stopped** shows the number of processes ending and releasing resources. The stopped processes send a termination message to the **parent process**. The process created by the kernel in Linux is known as the “Parent Process.” All the processes derived from the parent process are termed as “Child Processes.”
    
5.  **Zombie** shows the number of processes waiting for its parent process to release resources. Zombie processes usually mean an application or service didn't exit gracefully. Having a few zombie processes is not a problem. 
    

The top command gives detailed insight on usage for an IT individual to gauge the availability of resources on a system. 

# Key Takeaways

Computers need to balance the resources used with the resources that are free. Ensuring that the CPU is not overused means that a system will run with few issues. 

-   The load in Linux is calculated by adding 1 for each process that is running or waiting to run. 
    
-   Monitoring the average load of Linux allows an IT professional to identify which processes are running to determine what to end in order to balance the system. A balanced system runs with fewer problems than one that is using too high of a percent of resources. 
    
-   The load average uses three time lengths to determine the use of the CPU: one minute, five minutes and fifteen minutes. 
    

The top command can give detailed information about the resource usage of tasks that are running or waiting to run.

#linux #process-management #resource-management #course3-module5 