# Azure CLI - To stream logs live in Cloud Shell, use the following command: 

az webapp log tail --name infrastructure --resource-group Infrastructure

https://infrastructure.azurewebsites.net

# Access log files

Linux/container apps: https://<app-name>.scm.azurewebsites.net/api/logs/docker/zip
Windows apps: https://<app-name>.scm.azurewebsites.net/api/dump

https://infrastructure.scm.azurewebsites.net/api/dump