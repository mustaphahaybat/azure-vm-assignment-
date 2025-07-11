# Azure Virtual Machine and Azure File Share Assignment

## Student
Mustafa Haybat

## Assignment Overview
This project involved creating and configuring an Azure Virtual Machine (VM) using a free Azure account. I connected to the VM remotely via RDP, set up an Azure File Share, and mounted it on the VM to enable persistent storage and file sharing.

The main steps completed were:

- Creating a resource group and virtual machine with recommended settings (Premium SSD disk, public IP, and security rules for RDP access)
- Connecting to the VM using Remote Desktop Protocol (RDP)
- Creating an Azure Storage Account and Azure File Share
- Mapping the Azure File Share as a network drive on the VM using PowerShell commands
- Testing the connection and ensuring persistent access to the file share

## Screenshots
Screenshots documenting each step, including VM creation, File Share setup, connection commands, and mapped network drives, can be found in the `img` folder.

## Azure File Share Usage
I successfully created an Azure File Share named `assignmentshare` within my storage account and mapped it to the VM as the Z: drive using PowerShell. This allowed me to create, read, and delete files on the shared storage from the VM.

## Challenges and Solutions
- **PowerShell Cmdlet Errors:** Initially, some PowerShell modules such as `NetSecurity` failed to load, causing command errors. Running PowerShell as Administrator resolved this issue.
- **Network Port 445 Accessibility:** Port 445 needed for SMB file sharing was sometimes blocked by the network firewall or ISP. I verified port accessibility using `Test-NetConnection` and ensured it was open.
- **Mapping Network Drive in CMD vs PowerShell:** Running the commands in the Command Prompt (CMD) led to errors due to syntax differences. Switching to PowerShell for execution fixed this problem.

---

If you want to check all the details and steps with screenshots, please visit my GitHub repository linked below.

Feel free to contact me for any questions or feedback.

---

🔗 GitHub Repo: [your-github-link-here]
