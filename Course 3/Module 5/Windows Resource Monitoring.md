-   Managing processes is useful in an IT support role when processes become unruly.
-   **Resource Monitoring Tool** in Windows provides information on system resources and process information.
-  **Process Explorer** is another tool in Windows that displays performance information for a specific process.
-   **PowerShell** command `Get-Process` can be used to get process information from the command line.
-   Use **pipes** to filter information to display only what you need.
	Example sort the top 3 processes:
	`Get-Process | Sort CPU -descending | Select -first 3 -Property ID.ProcessName.CPU`
-   Linux resource monitoring tools are also available.

# Supplemental Reading Resource Monitoring in Windows

For more information about system diagnostics processes in Windows, check out the link [here](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/get-process?view=powershell-5.1#outputs).

#process-management #resource-management #process-explorer 