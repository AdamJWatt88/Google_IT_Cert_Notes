-   To rename a file using command line in Bash, we use the **"mv"** or **"move item"** command.
-   The **move** command allows us to **rename files** without changing their directory location.
-   To demonstrate, we see a blue document on the desktop that needs to be renamed. Using the move command, the file is renamed to "yellow document".
```
	/* change blue document name to yellow document name */
	C:\Users\cindy\Documents> mv .\blue_document.txt yellow_document.txt
```
-   The move command also allows us to **move files from one directory to another**. In the demo, the yellow document is moved to the "My Documents" directory using the move command.
```
	/* move yellow document to the Documents folder */
	C:\Users\cindy\Documents> mv .\yellow_document.txt C:\Users\cindy\Documents
```
-   Wildcards can be used to move multiple files simultaneously. We see that the rest of the colored documents were moved to the "My Documents" directory using a **wildcard** with the move command.
```
	/* move yellow document to the Documents folder */
	C:\Users\cindy\Documents> mv *_document.txt C:\Users\cindy\Documents
```
#rename-files #move-files #course3-module1 