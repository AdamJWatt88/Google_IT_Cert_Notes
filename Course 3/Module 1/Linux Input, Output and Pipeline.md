-   In **Linux,** there are **three different I/O streams**: **Standard Out**, **Standard In**, and **Standard Error**.
-   **Standard Out** is used to send the output of a command to the screen by default, but it can be **redirected** to a file using the **>** operator. The **>>** operator can be used to **append** to an existing file instead of **overwriting** it.
	```
	echo woof > dog.txt
	echo woof >> dog.txt
	```
-   **Standard In** can be redirected to take input from a file instead of the keyboard. This is done using the **<** operator, and it works the same as the **"cat"** command in Linux.
	`cat < file_input.txt`
-   **Standard Error** displays error messages and can be redirected using the **2> operator**. The "2" denotes Standard Error.
	`ls /dir/fake_dir 2> error_output.txt`
-   The **/dev/null** file is a special file on Linux that can be used to filter out unwanted output.
	`less /var/log/syslog 2> /dev/null`
-   The **pipe command (|)** allows the output of one command to be used as the input of another command. This is similar to the Windows pipeline.
	`ls -la /etc | grep bluetooth`
-   The power of redirectors is evident when using the pipeline to quickly search for specific information in directories.

#bash #linux #redirect #append #standard-in #standard-out #standard-error #course3-module1 