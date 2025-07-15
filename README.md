<p align="center">
  <img src="https://github.com/user-attachments/assets/52fb680e-df8c-4430-a2b9-3dc6d43aa87f" width="300" />
</p>


# Install Microsoft Graph PowerShell

## Platform and Tools Used

- Microsoft Azure
- Web Browser
- PowerShell


## Objective

In this project, I will demonstrate how to install Microsoft Graph PowerShell. Microsoft Graph PowerShell is the official toolset to manage Entra ID (Azure AD) using PowerShell. It replaces older modules like AzureAD and gives you secure, scriptable access to identity, group, roles, policies, and more via Microsoft Graph API. It allows us to automate, manage, and interact with Entra ID using simple command-line instructions.

----

## To Install Microsoft Graph Powershell

 1. I opened PowerShell as an Administrator, then ran the command `Install-Module Microsoft.Graph -Scope CurrentUser -Verbose` and pressed **Y** to confirm the installation:

<img src="https://github.com/user-attachments/assets/5415c3d3-d43f-41f6-b0a8-088c4e5a30fa" width="650" alt="Screenshot 2025-07-14 193942" />

- Installing packages:
  
<img src="https://github.com/user-attachments/assets/376fffd1-531f-456e-9665-406ce9fad374" width="400" alt="Screenshot 2025-07-14 194232" />

2. I ran the command `Get-InstalledModule Microsoft.Graph` to confirm that it had been successfully installed:

<img src="https://github.com/user-attachments/assets/2ed8c33d-22f7-491e-a730-ef224e359167" width="600" alt="Screenshot 2025-07-14 194812" />

3. Next, I ran the command `Connect-MgGraph -Scopes "User.ReadWrite.All"` to connect to Microsoft Graph with delegated permissions to read and write user data. Once I ran the command, a browser window opened and I was prompted to sign in. I then proceeded to enter my Microsoft Entra ID credentials:

<img src="https://github.com/user-attachments/assets/2ffdd997-eea1-45bd-a924-5161d307f948" width="450" alt="Screenshot 2025-07-14 194953" />

4. To verify that I had successfully connected to Microsoft Graph, I ran the command `Get-MgUser`. As expected, I was able to view the existing users in my tenant through PowerShell:

<img src="https://github.com/user-attachments/assets/baf3a171-45f7-480b-ba1d-86fc10908963" width="600" alt="Screenshot 2025-07-14 202414" />






 



