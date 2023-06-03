-   To enable Internet Information Services (IIS) on Windows:
    -   Go to Control Panel > Turn Windows features on and off > Select "Web Server (IIS)" > Click "Add Features" > Install
-   To manage the IIS service:
    -   Right-click on the IIS entry in the Services Manager > Select Internet Information Services Manager
    -   Expand the server and select "Sites" to view the websites served by the service
-   To add a new website:
    -   Copy the website files to the inetpub directory (the default directory for serving websites with IIS)
    -   In the IIS Manager, right-click on the list of websites and select "Add Website"
    -   Fill in the required options, such as the website name, physical path, and port number for the website to run on
-   The default website runs on port 80, so a separate port (such as 8080) should be used for additional websites.
-   The success of the website installation and configuration can be tested by navigating to the website URL (e.g. localhost:8080) in a web browser.

#configure-services #windows #course4-module2 