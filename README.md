# HHA504_assignment_networking

## 1. Create a Virtual Private Cloud (VPC)
### GCP
### Azure
![Azure-VNet-Config](https://github.com/user-attachments/assets/bbcb7d46-9a28-48c4-a56e-597ab46c590e)
![Azure-VNet-Deployed](https://github.com/user-attachments/assets/9d672afe-1743-4c2f-8ffa-712fae5449ab)
- I went to the Azure portal and searched for virtual networks. Then, I pressed create and started setting the configurations. I made sure it was under the correct subscription and resource group. For the name, I wanted it to reflect the homework assignment and chose the region as East US. Next, for the secruity configurations, I did not select any of the options because I was scared to incur extra cost. Furthermore, for IP addresses, I left it as the default options of 10.0.0.0/16 and 10.0.0.0. And, I did not input any tags for the virtual network. After pressing create, the virual network successfully deployed.
### GCP


## 2. Assign a Dedicated IP
### GCP
### Azure
![Azure-IP_config](https://github.com/user-attachments/assets/8c72586b-853e-48fd-84dd-74ecdf58cca8)
![Azure-IP-deployed](https://github.com/user-attachments/assets/4b6d5474-4ffc-4b75-8c66-7d81b6b32b56)
- After creating the virtual network, I searched public IP addresses. I pressed create and started setting the configurations. I made sure it was under the correct subscription and resource group. For the name, I wanted it to reflect the homework assignment and I left the IP version as the default option of IPv4. Then, for SKU, I chose the basic option instead of standard and left the IP address assignment as static. For DNS name label, I was not sure what to input so I left it blank. Next, for idle timeout (minutes) and domain name label scope (preview), I left them as the default configurations of 4 minutes and none. After pressing create, the public IP address successfully deployed. However, I am not sure if I correctly completed this step because the instructions said to create the static public IP address for a resource within the VNet. And, I am not sure how to accurately execute the steps needed to precisely create the static public IP address for a resource within the VNet.
### GCP


## 3. Map IP to a Domain
### GCP
### Azure
![Azure-DNS-basic-config](https://github.com/user-attachments/assets/f1fa1c3f-1af0-4876-b227-9d23c44f4c29)
![Azure-DNS-zone](https://github.com/user-attachments/assets/afb5dac5-6e70-44a0-bdd3-48fbf5ab1c86)
- After creating the public IP address, I searched DNS zones. I pressed create and started setting the configurations. I made sure it was under the correct subscription and resource group. For the name, I wanted it to reflect the homework assignment. Then, when reaching the next page of DNS zone editor, it said to upload a DNS zone file and copy my DNS zone into line 1. I am not sure how to complete the prompts on the DNS zone editor page and the purpose of the prompts, though I would assume it would help map the IP address to a domain. I tried researching for resources that could help me complete this step, but I still remain confused on how to map the IP address to a domain using the DNS zone feature.

