## Resources
For more information about file and folder permissions in Windows, check out the link [here](https://technet.microsoft.com/en-us/library/cc732880(v=ws.11).aspx).

## Notes
-   **Simple Permissions**
    
    -   Sets of Special or Specific Permissions
    -   Checkbox for Special Permissions in Permission List
-   **Special Permissions**
    
    -   List of Special Permissions available in **Advanced Tab of Permission Setting**
    -   Enabling Simple Permissions enables fine-tuned Special Permissions
    -   Modifying Special Permissions like Basic Permissions
    -   Necessary for creating complex file/folder patterns
-   **Viewing Special Permissions in CLI**
    
    -   Use 'icacls' command
    -   Example: `icacls C:\Windows\Temp`
-   Example: Setting Permissions for C:/Windows/Temp
    
    -   All Users should be able to create files/folders
    -   Admins and Computer Account have full permissions
    -   IO descriptor indicates inheritance, but not for container
    -   User's group can write data, create folders and append data, and synchronous
    -   Creator Owner has full control of file/folder they own
-   Creating a File/Folder to Check Permissions
    
    -   Using output redirection, record output of 'icacls' to a file
    -   Example: 'icacls C:/Windows/Temp/example > icacls.txt'
    -   Check the output file to view permissions for created file/folder
-   Special Permissions and NTFS Decals can be complicated but powerful for customized sets of permissions.

#special-permissions #permissions #windows #course3-module2 