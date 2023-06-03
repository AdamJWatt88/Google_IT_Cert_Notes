-   To make **copies **of files and directories in **Windows GU**I, you can **right-click** and select **"Copy"** and **"Paste"**. Alternatively, you can use hotkeys, such as Ctrl-C for copy and Ctrl-V for paste.
-   In **PowerShell**, the command to copy something is **"cp"**, followed by the name of the file and the path of where to copy it.
-   To copy **multiple files** at once, you can use a wildcard character, such as `"*"` to select files based on a certain pattern. For example, to copy all files with a ".jpg" extension, you can use the command `"cp *.jpg"` followed by the path of where to copy them to.
	`C:\Users\cindy\Documents> cp *.jpg C:\Users\cindy\Desktop`
-   To **copy the contents of a directory along with the directory itself**, you need to use the **"-Recurse"** parameter with the **"cp"** command. You can also use the **"-Verbose"** parameter to output one line for each file being copied. 
	`C:\Users\cindy\Documents> cp 'Bird Pictures' C:\Users\cindy\Desktop -Recurse -Verbose`

#windows-CLI #recurse #verbose #copy #paste #course3-module1 