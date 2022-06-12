<img src="https://raw.githubusercontent.com/Sufi-Dev/weatherapi/Sufi-Dev-Test/weatherapi.png" >

## Project Info <img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/info.gif" width="30" height="30">
This web API is sample basic API that is designed to respond with weather data.
The API will have to be linked to CosmosDB., an Azure NoSQL database. The focus of this project is the automation of CI/CD pipelines.

## Project Map <img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/map.png" width="30" height="30">
1) **CI/CD piplines**: I used Azure DevOps to set up fully automated CI/CD piplines.<br>
   Checkout the code for the pipeline in [`azure-pipelines.yml`](https://github.com/Sufi-Dev/weatherapi/blob/main/azure-pipelines.yml)as well as the Docker file in [`Dockerfile`](https://github.com/Sufi-Dev/weatherapi/blob/main/Dockerfile)<br>
2) **Terraform**: I provisioned cloud infrastructued using terraform.<br>
checkout terraform files in the [`terraform`](https://github.com/Sufi-Dev/weatherapi/tree/main/terraform) directory.
```
tree ./terraform 
├── main.tf
├── modules
│   ├── compute
│   │   └── vm
│   │       ├── main.tf
│   │       ├── terraform.tfvars
│   │       └── variable.tf
│   ├── network
│   │   └── vnet
│   │       ├── maint.tf
│   │       └── variable.tf
│   ├── security
│   │   └── network_security_group
│   │       ├── maint.tf
│   │       └── variable.tf
│   └── storage
│       └── cosmosDB
│           ├── main.tf
│           └── variable.tf
├── outputs.tf
├── provider.tf
├── terraform.tfvars
└── variables.tf
```
3) **Ansible**: Configured the provisioned server using ansible playbook automatically after terraform completed building the infrastructure.
checkout ansible playbook in the [`ansible`](https://github.com/Sufi-Dev/weatherapi/tree/main/ansible) directory.

## Tools 🛠
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/azure.svg" alt="azure" width="40" height="20"/> Azure
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/terraform.svg" alt="azure" width="40" height="20"/> Terraform
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/linux.svg" alt="linux" width="40" height="20"/> Linux 
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/nosql.svg" alt="azure" width="40" height="20"/> NoSQL
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="20"/>Docker
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/ansible.svg" width="40" height="20" /> Ansible
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/git.svg" width="40" height="20" /> Git
<img src="https://raw.githubusercontent.com/Sufi-Dev/Sufi-Dev/main/icons/AzureDevOps.svg" width="40" height="20" /> Azure DevOps 

## Related Pojects 🔗
I deployed the same web API in a **Blue Green deployment** architecture. See the link below:<br>
[Automated cloud infrastructure deployment using Terraform based on (Blue Green) deployment architecture](https://github.com/Sufi-Dev/Blue-Green-Deployment)



