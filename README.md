Usage: ./checkrsh
The script utilizes the dpkg command to view installed packages and uses grep to search for the presence of the rsh-server package. If the rsh-server package is found, the script notifies the user, indicates non-compliance, and provides the option to uninstall the rsh-server package. If the package is not found, the script informs the user that rsh-server is not installed.

Usage: ./blockrsh 
Description
The script checks the /etc/ssh/sshd_config file for the presence of specific options related to security settings. If the required configurations are found, it informs the user that the system is secure. Otherwise, it prompts the user to make changes to the SSH server configuration.

Configurations Checked
PermitEmptyPasswords: Disabled (set to 'no')
PermitUserEnvironment: Disabled (set to 'no')

Usage: ./banner
The script checks if the exact approved Standard Mandatory DoD Notice and Consent Banner text is configured in the system. If the banner is configured correctly, it informs the user. If not, it notifies the user of a security issue and provides the option to apply the banner text.

Usage: ./0755
The script checks the current permissions of the /var/log directory and determines if they are set correctly. If the permissions are correct, it informs the user that the system is secure. If not, it notifies the user of a security issue and provides the option to configure the /var/log directory with the correct permissions.
