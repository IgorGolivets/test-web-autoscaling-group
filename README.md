# test-web-autoscaling-group
Azure autoscaling group scripts with web app

Runs with Azure CLI on the Jenkins (with azure service principal embedded and Azure CLI plugin):

az group create --name myResourceGroup --location eastus

az group deployment create --resource-group myResourceGroup --template-uri https://raw.githubusercontent.com/IgorGolivets/test-web-autoscaling-group/master/autoscale_nginx.json --parameters adminUsername=someusername adminPassword="somepassword123"

web app will be available by this link:
"http://test-web-app.eastus.cloudapp.azure.com"
