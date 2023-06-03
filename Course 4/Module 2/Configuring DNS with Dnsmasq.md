-   In large enterprise deployments, different programs serve each of the networking services covered in this module. In smaller set-ups, a centralized solution may be better.
- `dnsmasq` is a program that provides **DNS**, **DHCP**, **TFTP**, and **PXE** services in a simple package.
-   After installing `dnsmasq`, it is **immediately** enabled with the most basic functionality of providing a cache for DNS queries.
-   The `dig` command is used to **query DNS servers** and see their answers.
- To query a DNS server running on the local host for the address of a specific website (e.g., www.example.com, we can use the command `dig www.example.com @localhost`.
-   Running `dnsmasq` in **debug** **mode** provides more information about what is going on behind the scenes with the command `sudo dnsmasq -d -q`
-   `dnsmasq` can be used to **give authoritative answers** for a list of host names and IPs. The file format for this list is the same as the **/etc/hosts** file.
-   The `-H` parameter is used to tell `dnsmasq` to include the list of hosts being served.
-   `dnsmasq` **forwards queries** to the **configured DNS server** if it does not have the requested information.
-   The output for queries that `dnsmasq` cannot answer shows that it forwards the query to the configured DNS server and lists the result as NX domain, which means non-existent domain.
-   `dnsmasq` is a simple example of what a DNS server looks like in action.

#dnsmasq #dns-servers #query-dns-servers #configure-dns 


