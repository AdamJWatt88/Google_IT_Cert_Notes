-   To **add a user,** go to the **computer management tool** and under **local users and groups,** right-click and select new user.
-   Set a **username, full name, and a password**, making sure to set a default password and **check the box for the user to change the password** at the next logon.
-   To **remove** a user, simply **right-click** and select **delete**.
-   Usernames are unique, and even if you delete a user and give them the same username, they won't be able to access their old resources.
-   Adding and removing local user accounts from the **CLI** uses the same **'net'** command used to change passwords but with different parameters.
-   Use **'net user /add'** to add a new local user and **'net user /del'** to remove a local user.
-   To **add** a new local user with a prompt for a password, use 
	`net user username * /add`
-   Use `net user username /logonpasswordchange:yes` to flag a user's account as requiring a password change.
-   To create an account that requires a **password change at the first login**, use `net user username password /add /logonpasswordchg:yes`
-   Use **'Get-LocalUser'** to list user accounts.
-   To **delete** an account use the **/del** command
	`net user user /del`
-   Use **'Remove-LocalUser'** to **remove** a local user account.
	`Remove-Localuser user`
-   Knowing the patterns of CLI commands will help you discover new things and remember how to do things you haven't done in a while.

#windows #add-user #remove-user #passwords #windows-CLI #course3-module2 