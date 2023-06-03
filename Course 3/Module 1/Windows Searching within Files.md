-   Finding words in a text document is a common task, and most text editors have a **Ctrl-F**function for this purpose.
-   Windows has a service called the **Windows Search Service** that indexes files on the computer and compiles a list of names and properties into a database.
-   **By default**, the **Windows Search Service** can find files based on their **name**, **path**, **modification time**, **size**, or **other detail**s but **cannot search for words inside the files**.
-   The Windows Search Service can be **configured to search file contents** and their properties, but this increases the time it takes for the indexer to do its work.
-   To **configure the service** to index file contents, go to Control Panel > Indexing Options > Users > Advanced > File Types > Index Properties and File Contents > OK.
-   After changing the settings, the Windows Search Service will start to rebuild the index based on the new settings, and the user can use Windows Explorer to find files that contain a specific word in them.
-   **Notepad++** can also be used to **search for words in files**, and the user can press **Ctrl+Shift+F** to open the Find in Files dialog and specify the word to find and the files to search.
-   In **PowerShell**, the **Select-String** command can be used to find words or other strings of characters in files, and the user can search for a word in a file in their home directory or search through several files in a directory using pattern matching.
-   Being able to find a string in a file or a set of files is a critical skill in IT support work.

#powershell #notepad #index-files #search-within-files #select-string #windows #course3-module1 