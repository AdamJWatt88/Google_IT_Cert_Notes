-   When a GPO-defined policy or a preference fails to apply to a computer, it could mean that something that was created using a GPO to configure it is not configured on one or more computers.
-   The **first and most common type of GPO failure** is related to the way group policies are applied, **known as fast log on optimization**. It means that some GPO changes take longer to be automatically applied, and it **can be fixed by forcing all GPOs** to be applied immediately with `gpupdate/force`. If you want to be really thorough, you can run a `gpupdate/force/sync`
-   The **log on server environment variable** will **contain** the **name of the domain controller** that the computer used to log on. Remember that you can see the contents of the variable with this command in **PowerShell**, which is `$env:LOGONSERVER`
-  **Replication failure** is another reason that a **GPO might fail to apply as expected**. Changes made to Active Directory usually take place on a single domain controller and then replicated out to other domain controllers. If replication fails, different computers on the network can have different ideas about the state of Directory objects, like group policy objects.
-   To **check on the overall health of the group policy infrastructure**, use the **Group Policy Management Console** to look at the **Status tab**, which will summarize the Active Directory and assist vault replication status for the domain. **All domain controllers should be listed** under domain controllers with replication in sync.
-   **If you're trying to work out why a particular GPO isn't applying to a computer,** the first thing to do is to **run the resultant set of policy or RSoP**. You can use the **Group Policy Management Console**, or you can run a command on a computer directly to generate the report using the `gpresult /R` command in **Powershell**. To get a full report that can be opened in your browser use the `gpresult /H NAMEDFILE.html`command
-   **When running the RSoP report, look for the following**: Is the GPO that needs to be applied listed? Was it linked to an OU that contains the computer being troubleshooted? Is the GPO listed under applied GPOs or under denied GPOs? If it was denied, what was the denied reason? Did another GPO win for the policy or preference that is trying to be configured? Is the security filter set to something besides authenticated users? Is the WMI filter set correctly?

# Supplemental Reading for Group Policy Troubleshooting

# Group Policy Troubleshooting

This reading expands upon a previous topic on various approaches to troubleshooting common Group Policy problems. 

## Terminology

Important terminology used with Microsoft Windows Server Group Policies:

-   **Group Policy Object (GPO):** A set of Active Directory (AD) Group Policy configurations that controls the appearance and behaviors for groups of computer systems and/or groups of end users. 
    
-   **Group Policy Management Console (GPMC):** A console that is used to create, manage, edit, and link GPOs. The GPMC provides thousands of options for computer and user settings such as Control Panel items, Registry settings, and environmental variables. Policy settings are refreshed every 90 minutes, so changes are not applied immediately. The GPMC can be used to create GPOs that control registry-based policies and software installations, as well as options for:
    
    -   security
        
    -   maintenance
        
    -   scripts
        
    -   folder redirection
        
-   **Active Directory (AD) containers:** AD containers can be linked to GPOs. AD containers include:
    
    -   **Sites:** Physical sites or aspects of a network, which are linked to AD Domains. Can be used to group and connect geographically dispersed locations into the same domain. 
        
    -   **Domain:** A collection of objects in an AD network, such as computers, users, and groups. Can contain multiple AD Sites and be linked to multiple GPOs. 
        
    -   **Organizational Unit (OU):** Collectively groups end users, computers, groups, and/or other OUs. OUs can reflect an organization’s hierarchy and business divisions. For example, an organization might have separate OUs for executives, administration, accounting, IT, sales, marketing, vendors, etc. 
        
-   **GPOs process order:** Windows will apply GPOs in the following order: 1) The Local GPO 2) GPOs linked to Sites 3) GPOs linked to Domains 4) GPOs linked to OUs
    
-   **Resultant Set of Policies (RSoPs):** A report of AD Group Policy settings that indicates how all GPO settings are hierarchically inherited by end users and computers. RSoP reports can be collected for evaluation using RSoPs logging. 
    
-   **Windows Management Infrastructure (MI) and Windows Management Instrumentation (WMI):** MI is the next generation of WMI. However, both MI and WMI are fully supported by Microsoft and MI is backwards-compatible with WMI. MI/WMI provide the operations infrastructure and management data in Windows. They also are used for scripting administrative tasks to run on remote systems.
    

## Group Policy troubleshooting tools 

The following command line tools can be used for troubleshooting Group Policy issues:

-   **gpresult:** Displays the RSoP report or values for a computer and user account. This information can help to ascertain which configuration settings have been applied and which settings were overridden. A few of the switches available to the gpresult command include:
    
    -   **/s** _host_ - Displays the RSoP values of a remote computer.
        
    -   **/u** _user-account -_ Displays the RSoP values of an end-user.
        
    -   **/p** _password -_ Displays the RSoP values of an end-user password policy.
        
    -   **/r** - Displays the RSoP summary of applied GPOs.
        
    -   **/z** - Turns on verbose mode to display details of the RSoP applied settings.
        

-   **gpedit:** The Group Policy Editor, which is a robust tool for changing Registry settings related to the Control Panel, Settings, user profiles, system configurations, third-party software, and more. 
    
-   **gpupdate:** Command that can be used to force a new or edited GPO to be applied immediately using the /force switch. If the policy setting requires the users to logoff or reboot, the switches /logoff or /boot can be added to the command.
    

Additionally, system event logs are important tools for most Windows troubleshooting issues:

-   **Event Viewer and Windows Logs:** The Windows Event Viewer is an invaluable tool for viewing Windows Logs. These tools help IT Support specialists track system problems and events related to items like applications, user logins, security, and systems. To open the Windows Event Viewer, click on the Start menu and type “Event Viewer”. Any error messages or codes found in the logs can be investigated using the Microsoft Knowledge Base (support.microsoft.com), as well as through an internet search. The main Windows Logs include:
    

-   **System log:** Records Windows OS events like hardware conflicts, driver load failures, service load failures, network issues, and more.
    
-   **Application log:** Records application processes and utilities events/errors.
    
-   **Security log:** Records system security audit information.
    
-   **Setup log:** Records installation events and errors.
    

## Resources for more information

-   [Group Policy troubleshooting documentation for Windows Server](https://docs.microsoft.com/en-us/troubleshoot/windows-server/group-policy/group-policy-overview) -  Extensive troubleshooting guide for Group Policies. Topics can be accessed from the left side menu.
    
-   [Group Policy processing and precedence](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2003/cc785665(v=ws.10)?redirectedfrom=MSDN) - Additional information about GPO processing order and exceptions.
    
-   [Active Directory documentation](https://docs.microsoft.com/en-us/troubleshoot/windows-server/identity/active-directory-overview) - Extensive troubleshooting guide for AD. Topics can be accessed from the left side menu.
    
-   [Use Resultant Set of Policy logging to gather computer policy information](https://docs.microsoft.com/en-us/troubleshoot/windows-server/group-policy/use-resultant-set-of-policy-logging) - Microsoft article that provides information on how to use the RSoPs utility (Rsop.msc) to gather computer-specific policy information.
    
-   [Suggested hotfixes for WMI related issue on Windows platforms](https://docs.microsoft.com/en-us/troubleshoot/windows-server/admin-development/hotfixes-for-wmi-issues) - Provides information on symptoms and resolutions for WMI issues.
    
-   [How the Windows Time Service Works](https://docs.microsoft.com/en-us/windows-server/networking/windows-time-service/How-the-Windows-Time-Service-Works) - (from the video on troubleshooting Group Policies) Microsoft article that includes information on how to manually force a domain computer to resync. 
    
    -   [W32tm](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/ff799054(v=ws.11)) - Syntax for using the **w32tm /resync** command, which can be used to diagnose problems related to Windows Time.
        
-   [6.3.2.3 SRV Records](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-adts/c1987d42-1847-4cc9-acf7-aab2136d6952) - (from the video on troubleshooting Group Policies) Information from Microsoft on the SRV DNS Resource Record.
#group-policy-management-console #group-policy-objects #resultant-set-of-policy #RSOP #RSOP-report #troubleshooting #course4-module4 