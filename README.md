# RhelPEAS-NG
RHELpeas.sh - Privilege Escalation Enumeration Script for RHEL

Created by: Robert Harp

rhelpeas.sh is a lightweight, yet powerful enumeration script tailored specifically for Red Hat Enterprise Linux (RHEL) systems. Modeled after the popular linpeas.sh, this script focuses exclusively on RHEL distributions and provides an extensive assessment of privilege escalation vectors. Additionally, it checks for containerized, cloud, and Kubernetes environments, as well as any installed databases. rhelpeas.sh was created to run on RHEL systems the are secure and when linpeas.sh is restricted from running on those RHEL systems. 

Features

	•	Privilege Escalation Vectors:
	•	Identifies misconfigurations, weak file permissions, and setuid binaries.
	•	Detects services running with elevated privileges.
	•	Container and Cloud Awareness:
	•	Enumerates Docker containers and related configurations.
	•	Detects the presence of cloud environments (AWS, Azure, GCP).
	•	Kubernetes Environment Checks:
	•	Checks for exposed Kubernetes configurations.
	•	Identifies Kubernetes-related credentials and tokens.
	•	Database Enumeration:
	•	Discovers installed databases (e.g., MySQL, PostgreSQL, MongoDB, etc.).
	•	Checks for misconfigured database files or credentials.
	•	RHEL-Specific:
	•	Tailored checks for RHEL-based systems, ensuring high accuracy and relevance.

Installation

	1.	Clone the repository or download the script:
 	git clone https://github.com/rharp86/rhelpeas.git
  	cd rhelpeas
   
	2.	Make the script executable:
 	chmod +x rhelpeas.sh

Usage

Run the script as a user with limited privileges. For the best results, use it on a system you have legitimate access to as part of a security assessment or penetration test.

Basic Usage:

./rhelpeas.sh

Save Output to a File:

./rhelpeas.sh > rhelpeas-output.txt

Verbose Mode:

./rhelpeas.sh -v

Output

The script will generate a detailed enumeration report, highlighting potential privilege escalation vectors, including but not limited to:

	•	Misconfigured permissions.
	•	Vulnerable binaries.
	•	Exposed credentials and tokens.
	•	Docker, Kubernetes, cloud, and database-related risks.

Requirements

	•	RHEL-based system.
	•	Bash shell.

Legal Disclaimer

This script is intended for authorized use only. It is designed to assist security professionals in identifying misconfigurations and potential privilege escalation vulnerabilities in Red Hat Enterprise Linux systems. Misuse of this script can result in severe legal consequences. The author disclaims any liability for actions taken with this tool.

Contributing

Feel free to open issues or pull requests to improve RHELpeas.sh. Contributions are welcome!

License

This project is licensed under the MIT License. See the LICENSE file for details.
