-   To **search** for specific files within a directory, use the **-Filter** parameter in **PowerShell**.
-   The **-Filter** parameter filters the results for file names that match a specified pattern.
-   The **syntax** for the **-Filter** parameter is as follows:
	    `ls 'C:\Program Files\' -Recurse -Filter *.exe`
-  To search for executable files within a directory using the -Filter parameter, follow these steps:
    1.  Use the **ls command** to list the files within the directory.
    2.  Use the **-Recurse** parameter to search for files within any subdirectories of the directory.
    3.  Use the **-Filter** parameter with the pattern "*.exe" to match files with the .exe extension.
-  The asterisk **(*)** in the pattern means **"match anything"** , and the .exe is the file extension for executable files in Windows.
-   Using the -Filter parameter allows you to quickly and easily search for specific files within a directory.

#search-within-directories  #filter #powershell #windows #course3-module1 