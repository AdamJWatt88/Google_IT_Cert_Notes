-   **Combining powerfu**l tools in PowerShell to perform complex tasks is possible
-   In PowerShell, the **echo** is actually an **alias for Write-Output**.
-   PowerShell commands can take **input** and produce **output**, and they use **I/O streams** or **input/output streams** to do so.
-   Processes and Windows have **three different streams**: **standard in**, **standard out**, and **standard error**.
-   To change where the standard output goes, we use the **greater than symbol**, which is a **redirect or operator**.
	`echo woof > dog.txt`
-   To **append information** instead of **overwriting an existing file**, we use the **greater than**, **greater than operator**.
	`echo woof >> dog.txt`
-   To pass the output of one command to the input of another command, we use the **pipe operator**.
	`cat words.txt | Select-String st`
-   To **redirect** the standard **error stream** to a file, we use the **two greater than symbol (2>)**.
	`rm secure_file 2> errors.txt`
-   To **filter out error messages**, we **redirect** standard error to `$null`.
	`rm secure_file 2> $null`
-   Use Get-help about_redirection in PowerShell to see more detail

#input #output #redirect #IO-stream #standard-in #standard-out #standard-error #course3-module1 