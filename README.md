Server Configuration Script

Welcome to the Server Configuration Script! This script streamlines the initial setup of a Debian/Ubuntu server, covering essential tasks like password management, user creation, SSH configuration, and the installation of WireGuard VPN.
🛠️ Features

    Change Root Password: Secure your server by updating the root password.
    Create a New User: Easily create a new user and set their password.
    Configure SSH Access: Prevent direct root access via SSH for enhanced security.
    Install WireGuard: Set up WireGuard for a secure VPN connection.

🚀 Getting Started
1. Clone the Repository

If you haven’t already cloned the repository, use the following command:

bash

git clone git@github.com:NicoVirgo1990/secure_server.git
cd secure_server

2. Make the Script Executable

Ensure the script has executable permissions:

bash

chmod +x setup.sh

3. Run the Script

Execute the script with root or sudo privileges:

bash

sudo ./setup.sh

✨ What Does It Do?
Install WireGuard

    Updates the package list and installs WireGuard with a single command, ensuring your server is ready for secure VPN connections.

Change Root Password

    Prompts you to set a new password for the root user, enhancing your server’s security.

Create a New User

    Asks for a new user name and creates the user if it doesn’t already exist.
    Prompts for a password and sets it for the newly created user.

Configure SSH

    Modifies the SSH configuration to prevent direct root access, improving overall server security.
    Restarts the SSH service to apply the new configuration.

💬 Example Output

When you run the script, you might see output like this:

plaintext

Installing WireGuard...
[...installation output...]

Changing root password...
[Enter new root password]
Password successfully changed for root

Enter the name of the new user to create: <username>
Creating new user <username>...
User <username> successfully created

Changing password for user <username>...
[Enter new password for <username>]
Password successfully changed for user <username>

Modifying SSH configuration to disable root access...
SSH service successfully restarted

Script completed successfully

⚙️ Configuration Options

You can customize how the script handles remote repository interactions. Set up your Git configuration to manage diverging branches:

    Merge Changes:

    bash

git config pull.rebase false

Rebase Changes:

bash

git config pull.rebase true

Fast-forward Only:

bash

    git config pull.ff only

📝 Contributing

We welcome contributions! To contribute:

    Fork the repository.
    Create a new branch for your changes (git checkout -b feature-branch).
    Make your changes and commit them (git commit -am 'Add new feature').
    Push your branch (git push origin feature-branch).
    Open a Pull Request.

📜 License

This project is licensed under the MIT License. See the LICENSE file for details
