-   Understanding what happens underneath the hood when installing or removing software is important, especially for IT professionals.
-   It is possible to use tools to monitor the actions an installation executable takes, even if the source code is not available.
-   When an **MSI** file or an executable wrapping an **MSI** is used for installation, the Windows installer system uses the information stored in the **tables** in the **MSI database** to guide how the installation should be performed.
-   MSI files contain a combination of databases that contain installation instructions in different tables, along with all of the files, objects, shortcuts, resources, and libraries needed for the program to function.
-   The Windows installer keeps track of all the actions it takes and creates a separate set of instructions to undo them, which allows for users to uninstall the program.
-   **Orca.exe** is a tool provided by Microsoft that is part of the **Windows SDK** and can be used to edit or create Windows installer packages.
-   Understanding the complex processes that occur during Windows installation can be surprising, especially considering it is initiated by just a few clicks.

#windows #MSI #orca #course3-module3 