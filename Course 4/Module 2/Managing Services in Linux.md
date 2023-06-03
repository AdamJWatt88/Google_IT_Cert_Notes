-   As a **system administrator**, you need to know how to **manage running services**
-   The way to do this **depends on the operating system**, but the **concepts are the same**
-   NTP (Network Time Protocol) is a service that synchronizes machine clocks
-   Ubuntu installations include an NTP daemon that manages clock synchronization
-   To check if the NTP daemon is running in Ubuntu, use the command `service ntp status`
-   If the clock drifts, the daemon adjusts it in small increments to prevent sudden time changes that may affect other services
-   If the clock drifts more than 128 milliseconds, the daemon assumes something else is going on and won't interfere
-   To manually adjust the clock, use the `sudo date` command followed by the desired date and time
-   To stop and start the NTP service, use the commands `sudo service ntp stop` and `sudo service ntp start`
-   To restart the NTP service, use the command `sudo service ntp restart`
-   These same commands can be used to manage more complex services.

#services #manage-services #course4-module2 #linux 