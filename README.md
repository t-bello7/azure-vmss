# azure-vmss

Virtual machine scale sets allows you to create identical virtual machine. The number of VM instances can automatically increase or decrease based on scheduled conditions

## Walkthrough
- Create a resource group for the resources
![storage account](./images/resource-group.png)

- Create a Virtual Network with a defualt subnet
![storage account](./images/scale-set-vnets.png)

- Create a network security group accepting incoming ssh, http and https request from 
my computer ip address. Attach to virtual network
![storage account](./images/vmss-nsg.png)

- Create a Virual machine scale set with a mininmum of 1 instance and can auto scale to two instance 
![storage account](./images/scale-set-vmss.png)

- Create a load balance with public ip address
![storage account](./images/vmss-lb.png)

- Create network interfaces to attach to the VMs
![storage account](./images/vmss-nsg.png)


N:B I could only create a maximum of two instance on the VMSS because my student subscription only gives 3 public IP adresses
- one for the lb and the remaining two for the instances 


- SSH into the VM and installed apache server 