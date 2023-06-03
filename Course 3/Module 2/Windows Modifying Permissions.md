-   To give access to another user on your machine to view a folder with family pictures, follow these steps:
    
    1.  **Right-click** on the folder and select **"Properties**"
    2.  Click on the **"Security"** tab
    3.  Click on **"Edit"** to edit file permissions
    4.  Click **"Add"** to add a group or username
    5.  Enter the username and click **"Check Names"** to verify
    6.  Click on the username and check the allow boxes for the desired permissions
-   The **"deny"** checkbox is special because it generally takes precedence over the allow permissions. If you explicitly check the deny box for a user's username, even if the group has access to the folder, the user won't.
    
-   To **modify** a permission in the **CLI,** use the **iCacls** command. If using **PowerShell**, surround iCacls parameters with **single quotes** to prevent PowerShell from interpreting the parameter as code. If using **Command Prompt**, use** double quotes** for the path and remove the single quotes.
	```
		//Powershell command
		icacls 'C:\folder\' /grant 'Everyone:(OI)(CI)(R)'

		//Command prompt command
		icacls "C:\folder\" /grant Everyone:(OI)(CI)(R)
	```

-   To give **read** permission to a directory for the **"everyone"** group, use the command "iCacls directory/grant everyone OI CI R".
	`icacls 'C:\folder\' /grant 'Everyone:(OI)(CI)(R)'`
    
-   To give **read** permission to a directory for the **"authenticated users"** group, use the command "iCacls directory/grant authenticated users OI CI R". This group doesn't include guest users.
    `icacls 'C:\folder' /grant 'Authenticated Users:(OI)(CI)(R)'`
    
-   To **remove** permissions for a group, use the command "iCacls directory/remove group".
       `icacls 'C:\folder' /remove Everyone
-   Use the iCacls command to verify the permissions are set as intended.

#permissions #modifying-permissions #windows #powershell #command-prompt #course3-module2 