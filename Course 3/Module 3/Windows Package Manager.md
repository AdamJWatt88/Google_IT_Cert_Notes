-   **Package managers** make software installation, removal, update, and dependency management **easy** and **automatic**.
-   **APT (Advanced Package Tool)** is a package manager for **Ubuntu** operating system.
-   The normal way to install software on Windows involves searching, downloading, and running the installer, updating manually, and using the add/remove programs utility for removal.
-   Windows Installer can manage dependencies but not **central catalog installation** or **automatic updates**.
-   **Chocolatey** is a third-party package manager for Windows that lets you install Windows applications from the **command line**.
-   Chocolatey is built on PowerShell and lets you install any package or software from the public Chocolatey repository.
-   You can create your own private repository for internal company applications, and configuration management tools like **SCCM** and **Puppet** can integrate with Chocolatey.
-   Chocolatey supports several methods of software installation, including using the command line tool and the package management feature in PowerShell.
-   To **install** a package, use the `Install-Package` command line tool and specify the package name, and to **uninstall** a package, use the `Uninstall-Package` command line tool and specify the package name.
	```
	Install-Package -Name sysinternals
	Uninstall-Package -Name sysinternals
	```

#package-managers #chocolatey #APT #windows #course3-module3 