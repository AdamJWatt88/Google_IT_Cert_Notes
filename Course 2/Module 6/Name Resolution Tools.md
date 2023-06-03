-   Name resolution is important for the Internet to function properly.
-   Operating systems handle lookups, but IT support specialists may need to run queries themselves to troubleshoot.
-   **nslookup** is a common command-line tool available on Linux, Mac, and Windows.
-   A basic use of nslookup involves executing the command with a **hostname** to get the resolution result and the server used to perform the request.
-   nslookup also has an **interactive mode** that allows for setting additional options and running multiple queries.
-   In interactive mode, the **"server"** command followed by an address can be used to make queries with a specific server instead of the default name server.
-   The **"set type"** command can be used to explicitly request certain resource record types, such as** MX** or **TXT records**.
-   The **"set debug"** command can be used to display full response packets, including intermediary requests and their contents. This provides more detailed information, but the amount of data can be overwhelming.

#nslookup #name-resolution-tools #course2-module6 