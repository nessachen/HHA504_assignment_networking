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
- I went to namecheap and created a free domain name which required me to make an account and verify my eligibility. After completing the registration process, I made my main domain name nessachen.me and was then able to create a record for a subdomain with a host name and the IP address from GCP. 
4. Deploy Flask Application
![GCP-namecheap-domain](https://github.com/user-attachments/assets/da670217-f5f1-4b0b-8e86-e8f89270c853)
- I copied the flask application from the provided repo. When looking through the files in the repo, I saw that it was slightly different than the flask deployed during the class demonstration. I made sure to create the same files with the same organization as the repo to avoid encountering errors. Then, I followed the steps completed during the class demonstration to configure the SSH.
5. Configure Firewall Settings
![GCP-Firewall](https://github.com/user-attachments/assets/6ec5fd6f-9440-4bd9-b714-24ebe6f81643)
![GCP-Firewall](https://github.com/user-attachments/assets/24f06b1b-3ef4-48aa-b45e-a4edca8925ec)
- I created a firewall rule as demonstrated during class. I made the name to reflect allowing port 5007. I left the configurations as the default options until source IPv4 ranges. For source IPv4 ranges, I entered 0.0.0.0/0. Then, I selected TCP and put 5007 as the port.
6. Access Your Application via Domain
![GCP-access-domain](https://github.com/user-attachments/assets/24a6973d-fe5e-4687-bf15-e8dcf826c154)
  
## Azure 
