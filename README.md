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
<img width="1876" height="923" alt="Step 11 VM_1 1 14" src="https://github.com/user-attachments/assets/286394b2-ec56-4387-931e-cab5590e9a73" />
<br>
<br>
Within the networking tab, I double checked to make sure port 3389 was open. I also selected the delete the public IP and NIC with VM deletion.
<br>
<br>
<img width="1876" height="923" alt="Step 13 VM_1 1 16" src="https://github.com/user-attachments/assets/150f0451-b01c-446b-b9f0-a8b1c25260a7" />
<br>
<br>
I didn't need the VM running when not in use, so I made sure that to enable auto-shutdown, in order to keep the cost low.
<br>
<br>
<img width="1876" height="918" alt="Step 14 VM_1 2 1" src="https://github.com/user-attachments/assets/e4c13bdf-27c5-4ee7-9668-147ecd02fc24" />
<br>
<br>
Before finalizing, I made sure to check how much running the VM was going to cost.
<br>
<br>
<img width="1875" height="920" alt="Step 15 VM_1 2 2" src="https://github.com/user-attachments/assets/c62e3669-c070-4996-bfce-957ea998519b" />
<br>
<br>
After I hit create, I made sure to check that the deployment was a success. 
<br>
<br>
<img width="1873" height="923" alt="Step 16 VM_1 2 3" src="https://github.com/user-attachments/assets/9698130c-87c6-408c-8a46-6b50f8fe83ce" />
<br>
<br>
Double checked to make sure that the VM connected to the vnet and had it's public IP address, for remote access.
<br>
<br>
<br>

### Remote Desktop Connection
<br>
<br>
<img width="1876" height="923" alt="Step 17 VM_1 2 3" src="https://github.com/user-attachments/assets/82bec466-ba86-4b79-890b-87b6231813c1" />
<br>
<br>
Using my personal computer, I opened up Remote Desktop Connection
<br>
<br>
<img width="1920" height="1080" alt="RDP Step 2_1 2 6" src="https://github.com/user-attachments/assets/02b658fc-0e7b-40df-8f8c-350ad084ceb0" />
<br>
<br>
After successful RDP connection, I opened up the System Information to check all of the specifications of the VM
<br>
<br>
<img width="1920" height="1080" alt="RDP Step 3_1 2 7" src="https://github.com/user-attachments/assets/47c2793f-a850-42ba-b702-9e4bf251d6a5" />
<br>
<br>
Just to double check everything, I used "ipconfig" in the command prompt to double check the IP address.
<br>
<br>

### Resource Cleanup
<br>
<br>
<img width="1876" height="923" alt="VM Stop 1_1 2 8" src="https://github.com/user-attachments/assets/18e0155d-9f96-48be-b6b8-1757ba41dd42" />
<br>
<br>
Once I was done, I made sure to close out of RDP and manually stop (deallocate) the VM, to help save on the cost.
<br>
<br>
<img width="1873" height="921" alt="VM Stop 2_1 2 9" src="https://github.com/user-attachments/assets/1478d807-8e00-49bb-847b-cad1c8b79f58" />
<br>
<br>
I waited until the "Status" if the VM was "Stopped (deallocated).
<br>
<br>
<img width="1873" height="923" alt="VM Delete 1_1 2 10" src="https://github.com/user-attachments/assets/cfb26429-498f-497a-afb0-9330ee39ffd7" />
<br>
<br>
Since I was done with the VM, I decided to delete it to help keep the cost low.
<br>
<br>
<img width="1878" height="921" alt="RG Delete 1_1 2 10" src="https://github.com/user-attachments/assets/9063a8ea-f5bb-48a3-95a7-6f49003b7af8" />
<br>
<br>
Now that I am done fully with the entire virtual machine and everything with it, I decided to delete the Resource Group to make sure it doesn't accrue any additional costs.
<br>
<br>
<img width="1876" height="921" alt="RG Delete Finished_1 2 11" src="https://github.com/user-attachments/assets/ba9b480d-d257-4f90-98a8-d2d83c2785c8" />
<br>
<br>
I waited for a full confirmation of the Resource Group deletion.
<br>
<br>
<img width="1876" height="923" alt="RG Delete Confirmation It&#39;s Deleted_1 2 12" src="https://github.com/user-attachments/assets/f346d64a-b288-4021-8a86-e40d57a70f7b" />
<br>
<br>
As soon as I got the notification of the deletion of the RG, and everything along with it, I refreshed the page to make sure the RG was completely removed from the Resource Manager.
