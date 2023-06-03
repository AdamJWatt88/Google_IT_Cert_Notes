-   Packages of software often rely on other pieces of code, called **dependencies**, to function properly.
-   For example, a game might have a dependency on a physics engine and a rendering library.
-   A library is a package of useful code that someone else wrote, bundled together as a single unit.
-   In Windows, **shared libraries** are called **dynamic link libraries (DLLs)**, and they can be used by many different programs.
-   Windows applications typically have many dependencies located together in a single installation package, along with an **MSI** file that tells the installer how to put it all together.
-   In the past, updating shared libraries could cause issues (DLL hell), but modern Windows operating systems use **side-by-side assemblies (SXS)** to manage shared libraries and resources.
-   SXS supports access to multiple versions of the same shared library automatically, and dependencies are bundled together in installation packages.
-   You can use a **Windows Package Manager** to locate, install, and maintain the libraries and other dependencies that your installed software needs to use.
-   **PowerShell** is a command-line interface for Windows that includes many built-in **commandlets** (commands).
-   The PowerShell commandlet **Find-Package** can locate software along with its dependencies, and **Install-Package** can be used to install the software and dependencies.
-  When you want to use chocolatey to find your packages you need to first register it using the **Register-PackageSource** command
	`Register-PackageSource -Name chocolatey -ProviderName Chocolatey -Location http://chocolatey.org/api/v2`
-   **Chocolatey** is a package repository for Windows software packages that can be added as a package source in PowerShell.
-  To verify if the package is installed correctly you can use the **Get-PackageSource** command
-   To locate the package and its dependencies again with `Find-Package sysinternals -IncludeDependencies`

#windows #package-dependencies #course3-module3 