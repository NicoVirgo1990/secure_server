Server Setup Script

This script makes it easy to set up your Debian/Ubuntu server. It does the following:

    Changes the root password
    Creates a new user and sets their password
    Configures SSH to block root access
    Installs WireGuard VPN

How to Use
1. Clone the Repository

If you haven’t cloned the repository yet, do so with:

bash

git clone git@github.com:NicoVirgo1990/secure_server.git
cd secure_server

2. Make the Script Executable

Set the script as executable:

bash

chmod +x setup.sh

3. Run the Script

Execute the script with root or sudo privileges:

bash

sudo ./setup.sh

What the Script Does

    Installs WireGuard: Prepares your server for VPN use.
    Changes Root Password: Asks you to set a new password for the root user.
    Creates a New User: Prompts for a new user’s name and password.
    Configures SSH: Updates SSH settings to disable root login and restarts the service.

Example Output

When you run the script, you’ll see messages like this:

plaintext

Installing WireGuard...
[...installation output...]

Changing root password...
[Enter new root password]
Password changed for root

Enter the name of the new user: <username>
Creating user <username>...
User <username> created

Changing password for user <username>...
[Enter new password for <username>]
Password changed for user <username>

Updating SSH configuration...
SSH service restarted

Script completed successfully

Contributing

To contribute:

    Fork the repository.
    Create a new branch (git checkout -b your-branch).
    Make changes and commit (git commit -am 'Description').
    Push your branch (git push origin your-branch).
    Open a Pull Request.

License

This project is licensed under the MIT License. See LICENSE for details.

Thanks for using the Server Setup Script! If you need help, open an issue on our GitHub page.

This version keeps things simple and clear, making it easy to understand and follow.
