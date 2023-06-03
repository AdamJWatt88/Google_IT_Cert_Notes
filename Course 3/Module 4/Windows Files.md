-   In this video, we learn about **file data** and **file metadata** in the context of the NTFS file system format used in Windows.
-   NTFS uses the **master file table (MFT)** to keep track of file metadata and data. Each file on a volume has at least one entry in the MFT.
-   **Attributes** such as **file name**, **creation timestamp**, **read-only status**, **compression status**, and **location of the file data** are **stored** in the **MFT**.
-   When a file is created, an entry is added to the MFT, and when it is deleted, its entry is marked as free for reuse.
-   **Shortcuts** are another type of file in Windows, and they have a reference to some destination file or folder.
-   **Symbolic links** are **similar** to shortcuts but operate at the **file system level**. When you create a symbolic link, it points to the name of another file or entry in the MFT.
-   The operating system treats symbolic links like **substitutes** for the **original file** in almost every meaningful way.
-   **Hard links** are another type of link that points to the **file record number** in the MFT, **not** the **file name**.
-   With a hard link, you can change the file name of the original file, and the link will still work.

# Supplemental Reading on NTFS File System

 For more information about the NTFS file system, please check out the following links: [Master File Table](https://msdn.microsoft.com/en-us/library/windows/desktop/aa365230(v=vs.85).aspx), [Creating Symbolic Links](https://msdn.microsoft.com/en-us/library/windows/desktop/aa363878(v=vs.85).aspx), and [Hard Links and Junctions](https://msdn.microsoft.com/en-us/library/windows/desktop/aa365006(v=vs.85).aspx).

#shortcuts #hard-links #symbolic-links #course3-module4 