-   Sometimes you need to test connectivity at the **transport layer**
-   Two powerful tools for this are **Netcat** (on Linux/MacOS) and **Test-NetConnection** (on Windows)
-  The Netcat tool can be run through the **command nc** and **has two mandatory arguments**, a **host** and a **port**.
-   Running "nc google.com 80" tries to establish a connection on port 80 to google.com
-   If the connection succeeds, a blinking cursor appears, allowing you to send application layer data to the listening service
-   Using the **"-z" flag** with Netcat tells you if a connection to the specified port is possible
-   Using the **"-v" flag** with Netcat provides more useful output for human eyes
-   Test-NetConnection on Windows defaults to using **ICMP echo request** when run with only a host specified
-   Test-NetConnection can test connectivity to a specific port by using the **"-port" flag**
-   Netcat and Test-NetConnection are both very powerful tools with many functions beyond what is covered in this video see the [[Testing Port Conectivity Reference Guide]]

#netcat #test-netconnection #course2-module6 