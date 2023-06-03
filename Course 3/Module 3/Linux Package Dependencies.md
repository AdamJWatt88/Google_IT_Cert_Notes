-   Installing a package in Linux may require the installation of other packages or shared libraries, which are called **package dependencies**.
-   When installing a package using a **stand-alone package installer** like **dpkg**, it does not automatically install its dependencies.
-   Failure to install dependencies will result in dependency error preventing package configuration.
-   Example: sudo dpkg-i Google Chrome command shows an error message indicating that Google Chrome Stable cannot be installed due to dependency problems that require the installation of the **libappindicator1** package.
-   **Shared libraries** in Linux are similar to **Windows DLLs**, which are libraries of code that other programs can use.
-   Installing package dependencies one by one is time-consuming and tedious, especially when multiple dependencies are needed.
-   **Package managers** are software tools that automate the installation, removal, and management of packages, including installing package dependencies.
-   Package managers make package installation and removal easier by handling dependencies automatically.

#package-managers #package-dependencies #linux #course3-module3 