# SAFELINE-WAF-WITH-DVWA
This project sets up SafeLine WAF with DVWA to test how a web application firewall detects and blocks attacks. After installing SafeLine, I performed SQL Injection, Command Injection, and HTTP Flood tests on DVWA to observe the WAF’s response. The setup shows how SafeLine protects vulnerable applications using rules and different security modes.

🔧 SafeLine WAF Installation – Detailed Explanation

To begin the home-lab setup, SafeLine WAF was installed using the Automatic Deployment Script provided officially by SafePoint. SafeLine offers a one-command installation method that automatically downloads all required components, configures system dependencies, and deploys the WAF engine without requiring manual setup.

# ⭐ 1. Downloading and Running the Installation Script

* SafePoint provides a pre-built installation script that can be executed directly from the terminal. This script:

* Fetches the latest SafeLine packages

* Installs necessary runtime dependencies

* Configures network listeners

* Installs system service entries

* Starts the WAF engine automatically

* The typical installation command looks like this:

* COMMAND (AUTOMATIC DEPLOY) -> bash -c "$(curl -fsSLk https://waf.chaitin.com/release/latest/manager.sh)" -- --en)

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-11-28%20160420.png?raw=true)



# ⭐ 2. Automated Environment Configuration

During installation, SafeLine performs several automated checks:

* Verifies OS compatibility (Ubuntu/CentOS)

* Installs required packages (Docker, container runtime, certificates)

* Sets up required folders under /opt/safeline

* Pulls SafeLine WAF engine containers

* Configures network ports for:

   * 9443 → Web Dashboard

   * 80/443 → Reverse Proxy Entry Points

* Enables firewall rules if required

This automation ensures the WAF can run with minimal admin intervention.

# ⭐ 3. Automatic Credential Generation

Once installation finishes, SafeLine prints out initial login credentials, typically containing:

* Admin Username

* Admin Password

* Dashboard URL (https://<your-ip>:9443)

These credentials are generated only once during installation and are required to access the SafeLine management panel.

# ⭐ 4. Deploying the WAF Dashboard

After installation, the SafeLine dashboard becomes accessible at:

=> https://<your-ip>:9443


At this stage:

* The WAF backend, rule engine, and management services run as Docker containers.

* HTTPS is enabled by default using system-generated certificates.

* The dashboard provides an interface to manage:

    * Protection rules

    * Traffic statistics

    * Attack logs

    * Custom policies

    * Authentication blocks

    * Dynamic protection settings

# ⭐ 5. Verifying Installation

To ensure installation completed correctly, the following commands can be used:

** COMMAND : sudo docker ps


Expected containers include:

* safeline-mgt

* safeline-luigi

* safeline-pg

* safeline-chaos

* safeline-detector

* safeline-tengine

If all containers are UP, SafeLine is fully operational.

# ⭐ 6. Ready for Integration with DVWA

* Once installation is complete, the next step is connecting SafeLine WAF with DVWA by:

* Configuring DVWA’s IP/Domain inside SafeLine

* Setting SafeLine as the reverse proxy

* Routing attacker traffic through SafeLine to observe:

   * Attack detection

   * Blocking

   * Logging

   * Auto-protection modes
