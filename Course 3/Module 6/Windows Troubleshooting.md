
In an IT support environment, it’s common to come across issues that you can resolve using the log analysis tools. These tools can help with application crashes, a slow boot or startup, application hangs, or unexpected reboots.  In this reading you will learn how to resolve application crashes through the Windows’ graphical user interface (GUI) and your system log files. 

## Solving the problem

When you begin to troubleshoot an IT issue, you should begin by researching the root of the problem.You might ask yourself these questions:

-   Is the problem unique to one computer or all computers on the network? 
    
-   Does the problem affect a single user or all users? 
    
-   Is the problem related to a particular application? Is that application up-to-date?
    

Information in your system and application logs can help you answer these questions.

Once you have figured out the problem, decide how you are going to fix it. You first attempt at fixing it might not be the right solution. This is okay and you are keeping the problem-solving process moving forward and helping to develop your technical troubleshooting skills.

After you have solved the issue and have figured out how to fix it, educate others on your team and in your company about what you discovered. Educating others about IT issues that are happening will help prevent them from happening again.

It’s also important to document your solution to a problem. Many organizations have a structured documentation process in place for IT. This documentation is a place for you to record the issues you have encountered and the solutions you discovered.  If they don’t already have a documentation system, it is an opportunity to create a documentation system for your company and follow it. Documenting issues that arise, and solutions to those issues, will save the company and other IT support professionals time and resources in the future.

## An example scenario

Consider this situation: One of the commonly-used software applications at your company continuously crashes around the same time every day. You use information in the Windows log files to investigate the issue and see events as they happen live. There are several types of logs you may analyze. A good way to start is by analyzing the system and application logs.

### Accessing logs through the Windows GUI tool

In Windows you can access logs through the GUI using the Event Viewer tool. You can launch the Event Viewer through the Windows start menus or by typing eventvwr.msc from the run box. The Event Viewer records a lot of information about the system. With a custom view, you can create a filter that will look across all the event logs and focus the view on just the information you're interested in. 

In the scenario above, you’re interested in a crash event that happens around the same time every day. You may create a custom view to filter only events that happen around the time of your crash event. Select the “error” and “critical” checkboxes to limit the view to include crash events. You can also select specific logs to view. The system log is a good place to start. Name the new view and save it for future reference.

![Image of Event Viewer’s “Create Custom View” interface, for specifying filtering parameters.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/oDOJzTZkRr2aZvjg2vcawQ_df1eaf8ab7b940baa3b63929e8c473f1_4_yjV5vFHJjjvZS4ov56A9_EwKN0qfvT6W_6xGunRZ2c1ffo7Kq_jCizrGLVniztSlwQugjooMp4gbPi5oe5ZFdCfzOxVghcHMGKaV759-DLsrE-fcy7X05D0MrL3dUj4M8GUcHuyML63YJ06HPdC2wdkYPVEY3rdj5ErRl04odOATmycdqHVZgVZn7J5bM?expiry=1683417600000&hmac=fA-8mTTmOU6TQgWvTMwBNto8R6dOBcGmTTACsJ2CFK0)

### Interpreting the log file

Once you have accessed your logs and focused on those parts that contain information most relevant to your crash event, you can examine the logs to find the root cause of the issue. Since you’re concerned with the crash of a specific application, you might scan the log file for the word “error” or the application name. Check the timestamps of these error logs for crashes that happen around the time that you suspect your crashes are happening. These parts of your system logs are most likely to offer clues about what’s causing your problem and how to fix it.

You may have to examine the logs a few times to collect the data you need. You may also have to try multiple different solutions before finding the right one. Then once you have, you can document it so others don’t have to go through the same process again. 

## Key takeaways

Good problem solving skills will help expedite the troubleshooting process and increase productivity.

-   When faced with a problem, analyze the situation to determine what steps to take.
    
-   There are two key tools that can help you resolve application errors:
    

1. Access to logs through the Windows GUI

2. Log analysis

-   After reaching your conclusions about a problem, communicate your findings.
    
-   Document your solution to every problem.