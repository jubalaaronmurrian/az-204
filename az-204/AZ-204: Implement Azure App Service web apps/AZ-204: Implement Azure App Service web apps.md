# App Service on Linux

az webapp list-runtimes --os-type linux
az webapp list-runtimes --os-type windows

# Find outbound IPs

az webapp show --resource-group Infrastructure --name infrastructure --query outboundIpAddresses --output tsv
az webapp show --resource-group Infrastructure --name infrastructure --query possibleOutboundIpAddresses --output tsv

# Find Groups

az group list
az group list --query "[].{id:name}" -o tsv