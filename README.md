# Secure Server and WireGuard Configuration Scripts

This repository contains two scripts designed for server security and VPN configuration.

## Script 1: `secure_server`

The `secure_server` script performs the following tasks:
1. **Disables Root Access via SSH:** Modifies SSH configuration to prevent root login.
2. **Changes Root Password:** Prompts the user to set a new root password.
3. **Creates a New User:** Generates a new user and prompts for the user's password.
4. **Installs WireGuard:** Automatically installs WireGuard VPN software.

### Usage

1. Make the script executable:
    ```bash
    chmod +x secure_server
    ```
2. Run the script with root privileges:
    ```bash
    sudo ./secure_server
    ```

## Script 2: `wireguard_setup`

The `wireguard_setup` script configures WireGuard with a simple client-server setup:
1. **Generates Configuration Files:** Creates basic configuration for both server and client.
2. **Includes Preshared Key:** Automatically generates and includes a preshared key in the configurations.
3. **Endpoint Placeholder:** The user must manually insert the server endpoint into the client configuration.

### Usage

1. Make the script executable:
    ```bash
    chmod +x wireguard_setup
    ```
2. Run the script with root privileges:
    ```bash
    sudo ./wireguard_setup
    ```

3. **Complete the Setup:**
    - Open the client configuration file (`wg-client.conf`) and insert the server endpoint (IP/hostname) into the `[Peer]` section.

## Prerequisites

- **`secure_server`** requires sudo privileges to modify system settings and install packages.
- **`wireguard_setup`** requires sudo privileges to configure network settings and create configuration files.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or issues, please open an issue on this repository or contact [info@kamesystem.com](mailto:info@kamesystem.com).

