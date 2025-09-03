# Creating a Virtual Machine in Microsoft Azure

This guide explains how to create a **Windows Server 2019 Datacenter VM** in Azure.  

## Steps

### 1. Navigate to Azure Portal
Go to the [Azure Portal](https://portal.azure.com/) and search for **Virtual Machines** in the Marketplace.  

---

### 2. Basic Configuration
- **Subscription**: `CloudAcademyLabs Prod 2`  
- **Resource group**: `cal-3296-c14`  
- **Virtual machine name**: `ca-lab-vm`  
- **Region**: `(US) West US`  
- **Availability options**: `No infrastructure redundancy required`  
- **Security type**: `Standard`  
- **Image**: `Windows Server 2019 Datacenter Server Core - x64 Gen2`  

📷 Screenshot:  
<img width="1878" height="979" alt="Screenshot 2025-08-17 153737" src="https://github.com/user-attachments/assets/0a24a318-d06b-4989-99b7-1829f8f90f44" />


---

### 3. Disk Configuration
- **OS disk size**: `127 GiB (default)`  
- **OS disk type**: `Standard SSD (locally-redundant storage)`  
- **Delete with VM**: ✅ Enabled  
- **Key Management**: `Platform-managed key`  

📷 Screenshot:  
<img width="1888" height="981" alt="Screenshot 2025-08-17 153930" src="https://github.com/user-attachments/assets/86997353-da19-4719-beae-96b1be99a598" />


---

### 4. Networking Configuration
- **Virtual Network**: `(New) vnet-westus (cal-3296-c14)`  
- **Subnet**: `(New) snet-westus-1`  
- **Public IP**: New public IP assigned  
- **NIC Network Security Group**: `Basic`  
- **Inbound Ports**: `RDP (3389)` allowed  

📷 Screenshot:  
<img width="1903" height="969" alt="Screenshot 2025-08-17 154032" src="https://github.com/user-attachments/assets/738be229-43ac-432a-be83-e2cbbebe01ab" />


---

### 5. Deployment
Once validated, click **Review + Create**. After deployment is complete, you will see the confirmation page with all resources created.  

📷 Screenshot:  
<img width="1887" height="1073" alt="Screenshot 2025-08-17 154534" src="https://github.com/user-attachments/assets/47fa0efb-eaa4-4195-9cad-4ee6a9f15659" />


---

## Final Notes
- This VM will be deployed under the selected resource group and subscription.  
- You can later connect via RDP or SSH depending on the OS and configuration.  

