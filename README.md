# HHA504_assignment_networking

## GCP
1. Create a Virtual Private Cloud (VPC)
![](https://github.com/user-attachments/assets/e019ddfa-9085-4c82-9e09-b9197b4bccc1)
![GCP-Vnet-config](https://github.com/user-attachments/assets/01c54d67-8419-4829-baf4-44011d9a3f0c)
![GCP-Vnet-config](https://github.com/user-attachments/assets/cdbd4fe7-6ce7-46ef-a633-10c9a3498251)
![GCP-Vnet-config](https://github.com/user-attachments/assets/98c0b126-2420-476b-a9d4-4434abac3106)
- I went to GCP and searched for VPC networks. I pressed create and started setting the configurations. For the name, I wanted it to reflect the homework assignment. I left MTU as its default option of 1460 and subnet creation mode as its default option of custom, while leaving private IPv6 address settings checkbox as unselected. Next, for subnets, I set the name to reflect the homework assignment and chose the region as east US. I left the IP stack type as IPv4 and made the range as 10.0.0.0/16. For the remaining options of private google access, flow logs, and hybrid subnet, I left them all as the default option of off. In the firewall rules section, I did not select any of the options because I was not sure what they implied and thought it was best to leave it untouched. Furthermore, for dynamic routing mode, I left it as regional and chose the default option of legacy for best path selection mode. After pressing create, the VPC network was successfully deployed.
2. Assign a Dedicated or Dynamic IP
![GCP-VM-IP](https://github.com/user-attachments/assets/1ebcf7df-2c6f-4db5-8cb5-7820240afeb5)
![GCP-VM-IP](https://github.com/user-attachments/assets/4e14a295-9695-4e2d-883a-c4db544d31d7)
![GCP-VM-IP](https://github.com/user-attachments/assets/2891e577-e6c2-4aab-a83b-a3510c31a83f)
![GCP-VM-IP](https://github.com/user-attachments/assets/4d692d71-1110-4f16-a7e9-b68c4e0889dd)
![GCP-VM-IP](https://github.com/user-attachments/assets/0d23ed17-184e-4cb7-9750-32d44fe3f72a)
![GCP-VM-IP](https://github.com/user-attachments/assets/c448440e-6ad6-4fdb-b2a8-dc9490d01003)
- After creating the VPC network, I went to create the VM instance as we learned in class and I realized the pages to set configurations looked different than before. For the name, I wanted it to reflect the homework assignment and I chose a east US region. I left any as the option for zone and standard as the option for VM provisioning model. Next, I did not change the series and left it as E2 but changed e2-medium to e2-micro. Under OS and storage, I made sure to change the image type to Ubuntu. For networking, the layout of the page appears different than before. I am assuming it is due to creating the VPC network in the previous step. I selected the options of allowing HTTPS and HTTP traffic for firewall while leaving the other configurations as unselected until network interfaces. I was permitted to choose the dropdown and select the VPC network and subnetwork created in the previous step. It was really interesting how in the same section I was also able to reserve a static external IP address and I made the name of the static external IP address reflect the homework assignment. After that, for the remaining fields, I left them either as the default options or as unselected and then pressed create, which allowed for successful deployment.
3. Map IP to a Domain Acquired via GitHub Student Pack
![GCP-namecheap-domain](https://github.com/user-attachments/assets/e3d2e4fc-4f45-4315-b3cf-68bb4099a67f)
- I went to namecheap and created a free domain name which required me to make an account and verify my eligibility. After completing the registration process, I made my main domain name nessachen.me and was then able to create A Record for a subdomain with a host name and the IP address from GCP. 
4. Deploy Flask Application
![flask](https://github.com/user-attachments/assets/da670217-f5f1-4b0b-8e86-e8f89270c853)
- I copied the flask application from the provided repo. When looking through the files in the repo, I saw that it was slightly different than the flask deployed during the class demonstration. I made sure to create the same files with the same organization as the repo to avoid encountering errors. Then, I followed the steps completed during the class demonstration to configure the SSH.
5. Configure Firewall Settings
![GCP-Firewall](https://github.com/user-attachments/assets/6ec5fd6f-9440-4bd9-b714-24ebe6f81643)
![GCP-Firewall](https://github.com/user-attachments/assets/24f06b1b-3ef4-48aa-b45e-a4edca8925ec)
- I created a firewall rule as demonstrated during class. I made the name to reflect allowing port 5007. I left the configurations as the default options until source IPv4 ranges. For source IPv4 ranges, I entered 0.0.0.0/0. Then, I selected TCP and put 5007 as the port.
6. Access Your Application via Domain
![GCP-access-domain](https://github.com/user-attachments/assets/24a6973d-fe5e-4687-bf15-e8dcf826c154)
  
## Azure 
1. Create a Virtual Private Cloud (VPC)
![Azure-Vnet-config](https://github.com/user-attachments/assets/5cd0815e-8e73-4ac3-b538-6587107f12b5)
![Azure-Vnet-config](https://github.com/user-attachments/assets/e4c31a7f-81ca-463e-99b8-165b834d5db4)
![Azure-Vnet-config](https://github.com/user-attachments/assets/9b2b80df-c31a-4329-b588-96172cc7ee43)
- I went to the Azure portal and searched for virtual networks. I pressed create and started setting the configurations. I made sure it was under the correct subscription and resource group. For the name, I wanted it to reflect the homework assignment and chose the region as East US. Next, for security configurations, I did not select any of the options because I was scared to incur extra costs. Furthermore, for IP addresses, I left it as the default options of 10.0.0.0/16 and 10.0.0.0-10.0.0.255/24. And, I did not input any tags for the virtual network. After pressing create, the virtual network was successfully deployed.
2. Assign a Dedicated or Dynamic IP
![Azure-IP_config](https://github.com/user-attachments/assets/8c96f0dc-db0d-4e0e-8a49-4784130e58f9)
![Azure-IP_config](https://github.com/user-attachments/assets/679e63f5-68dd-474b-9369-89ce6fbe0d02)
![Azure-IP_config](https://github.com/user-attachments/assets/2bfacbb6-c050-4b5a-977c-9c318272e8ce)
![Azure-IP_config](https://github.com/user-attachments/assets/323e371f-0b34-4211-b302-00849f4f0a9d)
- After creating the virtual network, I searched public IP addresses. I pressed create and started setting the configurations. I made sure it was under the correct subscription and resource group. For the name, I wanted it to reflect the homework assignment and left the region as the default option of East US. For the remaining fields of the basics section, I left them as the default options. But, for DNS name label, I was not sure what to input so I left it blank. Next, in the sections of DDoS protection and tags, I did not select any options or input any information. After pressing create, the public IP address was successfully deployed.
![Azure-VM-IP](https://github.com/user-attachments/assets/cf5af4da-66e3-4936-b8d7-46e448765760)
![Azure-VM-IP](https://github.com/user-attachments/assets/e88c8346-e59d-47bc-902f-a334f56df630)
![Azure-VM-IP](https://github.com/user-attachments/assets/2d94672b-e91d-4c17-9c48-8a49781cf5f5)
![Azure-VM-IP](https://github.com/user-attachments/assets/13ed7cb6-b381-4cf3-805f-a2f35bb16769)
![Azure-VM-IP](https://github.com/user-attachments/assets/bdb6c05b-bb86-4097-8798-bcefd0b89b8d)
- After creating the public IP address, I searched for virtual machines. For the basic settings, I made sure it was under the correct subscription and resource group. I started by creating the name of the virtual machine to reflect the homework assignment and chose east US as the region. I left availability options, zone options, and availability zone as their default options. By choosing standard as the security type and Arm64, I was able to select a Ubuntu server as the image and standard_b2pts_v2 - 2 vcpus 1 GiB memory as the size. For the administration account settings under the basic settings, I changed the authentication type to password, which I proceeded by creating a username and password. I selected all of the available options of HTTP, HTTPS, and SSH for the inbound port rules. Next, I did not make any changes to the disks section. But for the networking section, I made sure to change the virtual network, subnet, and public IP to the ones created in the previous steps. Then, I did not make any changes to the management, monitoring, advanced, and tags sections. After pressing create, the virtual machine was successfully deployed.
3. Map IP to a Domain Acquired via GitHub Student Pack
![Azure-namecheap-domain](https://github.com/user-attachments/assets/bb0d066c-8bdd-41e9-9beb-8e8b3fe7a91e)
- I created a namecheap account when I started with the GCP portion of the assignment. Thus, I logged into my account and created A Record for a subdomain with the same host name (example) as the one from the GCP portion of the assignment, but inputted the IP address from Azure.
4. Deploy Flask Application
![flask](https://github.com/user-attachments/assets/da670217-f5f1-4b0b-8e86-e8f89270c853)
- This is the same flask used for the GCP portion of the assignment from the provided repo. I followed the steps completed during the class demonstration to configure the SSH, which was slightly different than how we did it for the GCP portion of the assignment. We were taught how to configure the SSH for the assignment through our local terminal by setting up the username and IP address for the virtual machine. Then, we needed to create a virtual environment on the local terminal, but the following steps remained the same as the GCP portion of the assignment.
5. Configure Firewall Settings
![Azure-Firewall](https://github.com/user-attachments/assets/23700cfb-3960-491c-878a-a4700fd7fbcc)
![Azure-Firewall](https://github.com/user-attachments/assets/d8d9b115-0a90-43ce-aea0-4a130293a4da)
- I configured the virtual machine firewall settings by clicking on the virtual machine I made for the assignment and went to the networking settings. I scrolled to the bottom of the page and pressed the create port rule. I changed the destination port ranges option to 5007 and adjusted the name of the port rule to allow-port-5007. For the remaining fields, I left them as the default options. To finalize the firewall settings for the virtual machine, I pressed add.
6. Access Your Application via Domain
![Azure-access-domain](https://github.com/user-attachments/assets/34d3d075-2bb1-4df4-a05c-9299a1cca6a1)
