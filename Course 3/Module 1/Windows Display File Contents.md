-   To open a file and view its contents in Windows GUI, double-click on the file and it will open in a default application, such as Notepad for text files.
-   To change the default application that opens files, right-click and click "Properties", then under "Open With", select another text editor like WordPad.
-   In **PowerShell**, we can view the contents of a file using the **"cat"** (concatenate) command, which dumps the whole file contents into the shell.
-   To view the contents of a file one page at a time, we can use the **"more"** command, which pauses once it fills the terminal window.
-   We can interact with the "more" program using different keys:** Enter** key advances by one line, **Space** key advances by one page, and **Q** key quits and goes back to the shell.
-   To view the first few lines of a file, we can use **"cat -head"** parameter to show the head of the file (first 10 lines by default).
	`cat document.txt -head`
-   To view the last few lines of a file (tail), we can use "tail" command, which shows the last 10 lines of a file by default.
	`cat document.txt -tail`

#windows-CLI #command-prompt #powershell #windows #course3-module1 