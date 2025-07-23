# Check-Point-Endpoint-Security-Client-Deployment---Technical-Report
This document provides a step-by-step guide for deploying the Check Point Endpoint Security Client on a Windows machine, including prerequisites, installation, policy configuration, and verification.

Table of Contents
Procedures i Followed
Step 1: Downloading the Endpoint Agent from Infinity Portal
Step 2: Transferring the Agent to the Windows Machine
Step 3: Installing the Endpoint Client
Step 4: Verifying Agent Connection in Infinity Portal
Step 5: Configuring Postpone Settings (Optional)
Step 6: Scanning for Threats and Verifying Deployment
Conclusion


Prerequisites
✅ Check Point Infinity Portal access (admin privileges)
✅ Windows machine (tested on Windows 10/11)
✅ Network connectivity to the Check Point server
✅ Downloaded KEXC agent file (e.g., Endpoint_Agent_Windows.exe)


Step 1: Downloading the Endpoint Agent from Infinity Portal
Log in to the Check Point Infinity Portal.
Navigate to Policy → Software Deployment.
Verify Threat Prevention capabilities (Anti-Malware, Anti-Ransomware, Behavioral Guard, Forensics).
Select the recommended version of the Endpoint Client.
Click Download to obtain the agent package.

(Screenshot: Downloading the Endpoint Agent from Infinity Portal)

Step 2: Transferring the Agent to the Windows Machine
Copy the downloaded KEXC file (Endpoint_Agent_Windows.exe) to the target Windows machine (via USB, network share, or email).

(Screenshot: Transferring the agent file to the Windows machine)


Step 3: Installing the Endpoint Client
Run the Endpoint_Agent_Windows.exe as Administrator.
Follow the installation wizard (default settings recommended).
The agent will automatically connect to the Check Point server.

(Screenshot: Installation progress and successful connection)

Step 4: Verifying Agent Connection in Infinity Portal
Go to Computer Management in the Infinity Portal.
Verify the client appears (e.g., DESKTOP-FGIRVN8).
Check the status (should be "Completed").

(Screenshot: Agent successfully connected and deployed)

Step 5: Configuring Postpone Settings (Optional)
To disable user postponement of installations:
Navigate to Policy → Global Policy Settings → Client Settings → Installation.
Uncheck "Allow users to postpone installation".
Save the policy.

(Screenshot: Modifying postpone settings in Global Policy)

Step 6: Scanning for Threats and Verifying Deployment
On the Windows machine, run a scan (Anti-Malware).
Check browser extensions (Chrome will show Check Point Agent Extension).
In Infinity Portal, refresh to confirm "Deployment Completed".

Conclusion
✅ Agent successfully deployed and connected to the Check Point server.
✅ Threat Prevention capabilities (Anti-Malware, Anti-Ransomware) are active.
✅ Compliance status confirmed in Infinity Portal.

