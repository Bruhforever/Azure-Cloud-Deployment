# Azure VM Deployment

## Description
This project demonstrated the deployment, configuration, validation and deletion of a Virtual Machine within Azure. The project involved creating a Windows Server environment, configuring required networking and access settings, and verifying remote connectivity through Remote Desktop Protocol.

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


### ***Resource Group Creation***
<img width="1872" height="919" alt="Step 1 Of Creation of RG_1 1 1" src="https://github.com/user-attachments/assets/7d3fa470-b629-4cd9-9204-1f391a9cd1d0" />
<br>
<br>
I started this project by first creating a resource group to keep all of my resources organized.
<br>
<br>
<img width="1882" height="926" alt="Step 2 Of Creation of RG_1 1 2" src="https://github.com/user-attachments/assets/7926c2a6-7c7a-4cbd-9133-ab473eeff0d8" />
<br>
<br>
I went with the name of "VM-Deployment-RG" to make sure that this resource group is easily identifiable.
<br>
<br>
<img width="1880" height="921" alt="Step 3 Of Creation of RG_1 1 3" src="https://github.com/user-attachments/assets/511167cc-fb5c-494e-8030-16735ba55a0a" />
<br>
<br>
I clicked on Resource Groups to make sure that the Resource Group was created successfully.
<br>
<br>
<br>
<br>

#### ***Virtual Machine Configuration***
<img width="1880" height="921" alt="Step 1 Of Creation of VM_1 1 4" src="https://github.com/user-attachments/assets/b6021adf-1425-47fd-99cb-eaf336061558" />
This project is about deploying a virtual machine within Azure, so naturally the next step is to start creating the virtual machine.
<br>
<br>
<img width="1880" height="921" alt="Step 2 Of Creation of VM_1 1 5" src="https://github.com/user-attachments/assets/43b9044b-60cc-418b-af28-e34e1d22c134" />
<br>
<br>
I made sure to select the Resource Group we just created, to make sure that all of the resources this virtual machine is going to be using are all in one easily identifiable place.
<br>
<br>
<img width="1880" height="921" alt="Step 3 Of Creation of VM_1 1 6" src="https://github.com/user-attachments/assets/bba84918-cb76-41c5-aaa1-8d147eb4e9ad" />
<br>
<br>
I wanted to continue the naming scheme that I started with the resource group, again to keep it easily identifiable.
<br>
<br>
<img width="1880" height="921" alt="Step 4 Of Creation of VM_1 1 7" src="https://github.com/user-attachments/assets/f7e9bf26-3d2e-42fb-8649-4149c7b3a9ba" />
<br>
<br>
I was looking for a Windows Server edition, with a low amount of vram to keep the cost lower, while also having availability in the region I wanted it to be in.
<br>
<br>
<img width="1880" height="921" alt="Step 5 of Creation of VM_1 1 8" src="https://github.com/user-attachments/assets/a1309713-9ffd-475e-bdf8-fbb865d2bc89" />
<br>
<br>
I made sure to create an administrator account, with password to allow of Remote Desktop access.
<br>
<br>
<img width="1880" height="921" alt="Step 6 in Creation of VM_1 1 9" src="https://github.com/user-attachments/assets/c8160458-5c9b-4b9b-aa33-4965dc651369" />
<br>
<br>
I made sure to select "Allowed Selected Ports" with 3389 being the port open to allow for Remote Desktop access.
<br>
<br>
<img width="1880" height="921" alt="Step 8 VM_1 1 11" src="https://github.com/user-attachments/assets/cf7384de-3386-41d6-a001-d62cadc635ba" />
<br>
<br>
I left the disk sizes default for this project. I didn't need any more than that. I also made sure that the "Delete with VM" option was selected, for when I was done with the project as a precaution.
<br>
<br>
<br>
<br>

### ***Networking Configuration***
<br>
<br>
<img width="1880" height="921" alt="Step 9 VM_1 1 12" src="https://github.com/user-attachments/assets/3a062d97-ff7d-4ca0-a791-ea1f8f89001b" />
<br>
<br>
I made sure to create, and name with the same naming scheme, the VNET to still keep everything easily identifiable.
<br>
<br>
<img width="1880" height="921" alt="Step 11 VM_1 1 14" src="https://github.com/user-attachments/assets/6141e890-ef45-424d-a865-83910bcacd47" />
<br>
<br>
Within the networking tab, I double checked to make sure port 3389 was open. I also selected the delete the public IP and NIC with VM deletion.
<br>
### Deployment Validation

<br>
After deployment, I verified the virtual machine was running successfully. 

### Remote Desktop Connection

<br>
I used a personal computer to access the virtual machine.
I used ipconfig to check network information.

### Resource Cleanup

<br>
After validation through RDP, I disconnected and deallocated the virtual machine.
<br>
<br>

<br>
<br>
After testing was completed, I deleted the resource group to remove all Azure resources associated with the project.
