# PAN-2FW-PLB

Azure:
[![Deploy to Azure](https://azuredeploy.net/deploybutton.png)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmcrosstx%2FPAN-2FW-PLB%2Fmaster%2Fazuredeploy.json)

Azure US Gov:
[![Deploy to AzureGov](https://azuredeploy.net/deploybutton.png)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmcrosstx%2FPAN-2FW-PLB%2Fmaster%2Fazuredeploy.json)

This Template deploys two Palo Alto virtual firewalls to Azure using Managed disks. It also deploys an Azure Public and Private Load Balancer to go along with the firewalls.

The firewalls have 4 interfaces:
* Management
* Internal/VPN
* Trust
* Untrust

Requirements:

You will need to have a VNet already setup with the appropriate subnets you would like to use for each interface of the firewalls. You will also need to have the Resource Groups already provisioned.