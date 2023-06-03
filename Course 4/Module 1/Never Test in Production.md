-   **Production** refers to the parts of **infrastructure** where a service is **executed** and served to its users.
-   To **safely make changes** in production, always run them through a **test environment first.**
-   The **test environment** is usually a **virtual machine** running the **same configuration** as a production environment, but **without serving any users**.
-   For important services that need to keep running during a configuration change, have a **secondary or stand-by machine that is exactly the same as the production machine** but isn't receiving traffic from actual users until you enable it to do so.
-   For bigger services with many service providers, use **canaries**, a small group of servers to detect any potential issues in larger changes before pushing them out to the rest of the fleet.
-   Even for **minor changes** in production infrastructure, **always try them in a test instance first**.
-   How to set up a test environment depends on the size and importance of the service.

#production #test-environment #infrastructure #virtual-machine  #course4-module1 