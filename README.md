# test-web-autoscaling-group
Azure autoscaling group scripts with web app

Run with Azure CLI on the Jenkins 9with azure service principal embedded):

az group create --name myResourceGroup --location eastus

az group deployment create --resource-group myResourceGroup --template-uri https://raw.githubusercontent.com/IgorGolivets/test-web-autoscaling-group/master/autoscale_nginx.json --parameters adminUsername=jenkins adminPassword="jenkins!2345"

web app will be available by this link:
"https://test-web-app.eastus.cloudapp.azure.com"
