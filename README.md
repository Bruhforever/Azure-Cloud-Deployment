# Azure VM Deployment

## Description
This project demonstrated the deployment, configuration, validation and deletion of a Virtual Machine within Azure. The project involved creating a Windows Server environment, configured required networking and access settings, and verifying remote connectivity through Remote Desktop Protocol.

## Technologies and Utilities Used
- Microsoft Azure
- Azure Virtual Machines
- Azure Virtual Network
- Remote Desktop Protocol
- Windows Command Prompt

## Environments Used
- Microsoft Azure
- Windows Server 2025 Datacenter: Azure Edition
  
## Deployment Walkthrough


### Resource Group Creation
<img width="1878" height="920" alt="rg-creation_1 1 1" src="https://github.com/user-attachments/assets/83fc1a0d-8c34-4391-b404-0c43735b19e3" />
<br>
<br>
I created this resource group in Azure to organize the virtual machine resources.
<br>
<br>

### Virtual Machine Configuration
<img width="1872" height="918" alt="vm-name" src="https://github.com/user-attachments/assets/120281cd-dd24-4654-b88a-63c7febf37f7" />
<br>
<br>
I used the naming scheme VM-Deployment-VM to keep the Azure resources organized and easily identifiable.
<br>
<br>
<img width="1873" height="920" alt="vm-username" src="https://github.com/user-attachments/assets/97fe1736-e094-4e58-97ba-f8099c9fe954" />
<br>
<br>
I created a local administrator account to allow Remote Desktop Protocol access and validate virtual machine deployment.
<br>
<br>
<img width="1879" height="921" alt="RDP-Port-Open_1 1 4" src="https://github.com/user-attachments/assets/1151ee4a-526e-4597-a25e-2f47315bdbef" />
<br>
<br>
I verified the RDP port was selected during VM configuration to allow for Remote Desktop access.
<br>
<br>
<img width="1879" height="923" alt="Vm-Deployment-FULLSCREEN_1 2 2_1 2 1" src="https://github.com/user-attachments/assets/d828fb62-cd0c-4a94-ace3-0a75ae2c10e1" />
<br>
<br>
I verified the configuration before Azure deployed the Virtual Machine.

### Networking Configuration
<img width="1877" height="922" alt="Vnet-Creation_1 1 5" src="https://github.com/user-attachments/assets/b01c4d9c-ac6f-4edf-b21c-f3eec48135cc" />
<br>
<br>
I created a virtual network to provide connectivity to the virtual machine.

### Deployment Validation
<img width="1879" height="923" alt="VM-RunningWithIP_1 2 4" src="https://github.com/user-attachments/assets/e2b531e9-da57-47a4-b087-4cb62028d645" />
<br>
<br>
After deployment, I verified the virtual machine was running successfully. 

### Remote Desktop Connection
<img width="1920" height="1080" alt="RDP-Success_1 2 5" src="https://github.com/user-attachments/assets/a435f782-182f-453b-8000-696680861ff2" />
<br>
<br>
Used a personal computer to access the virtual machine.
Used ipconfig to check network information.

### Resource Cleanup
<img width="1876" height="922" alt="vm-deallocated_1 2 7" src="https://github.com/user-attachments/assets/3950d861-9373-408e-adf4-79a8425010ef" />
<br>
<br>
After validation through RDP, I disconnected and deallocated the virtual machine.
<br>
<br>
<img width="1876" height="923" alt="RG-Deleted_1 2 8" src="https://github.com/user-attachments/assets/64da4c04-7d76-4474-8e14-4412f226f8a8" />
<br>
<br>
After testing was completed, I deleted the resource group to remove all Azure resources associated with the project.
