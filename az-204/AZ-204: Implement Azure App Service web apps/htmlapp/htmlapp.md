# Exercise: Create a static HTML web app by using Azure Cloud Shell

mkdir htmlapp
cd htmlapp
git clone https://github.com/Azure-Samples/html-docs-hello-world.git

resourceGroup=$(az group list --query "[].{id:name}" -o tsv)
appName=az204app$RANDOM

cd html-docs-hello-world
az webapp up -g $resourceGroup -n $appName --html

## Update and redeploy the app

az webapp up -g $resourceGroup -n $appName --html