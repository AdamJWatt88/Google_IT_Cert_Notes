-   **Metadata** and **files** are organized into an **Inode** structure in Linux, similar to **Windows NTFSM FT records**.
-  **Inodes** don't store file data or name but **contain other file information**.
-   **Soft links**, also known as **sim links**, allow creating shortcuts to other files using file names.
-   **Hard links** point to **Inodes** stored in the **Inode table** on the file system, pointing to a physical location on disk.
-   If a file with hard links is deleted, other hard links will still work.
-   The **hard link count** of a file is indicated in the **third field of the ls -l details**.
-   To **create a soft link**, use the ln command with the -s flag.
	`ln -s test_file test_file_softlink`
-   To **create a hard link**, use the ln command without the -s flag.
	`ln test_file test_file_hardlink`
-   Hard links are useful for having the same file** stored in different places **without taking up additional space.
-   Soft links **can break** if a file is **moved**, while** hard links will still work**.
-   Soft links and hard links are used throughout the system.