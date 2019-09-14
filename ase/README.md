# Scenario

Create the following resources
* A new resource group
* A new virtual network
* Subnets for ASE, App Gw and APIM
* ILB ASE
* App Service Plan for ASE Isolated SKU
* App Gw + WAF in existing subnet
* APIM in existing subnet 
* Scripts for following
  * Configuring certificates (if required) on ASE and App GW
  * Connecting App Gw with APIM and directly to ASE as separate backends
  * Connecting APIM to WebApps exposing APIs 
  * webApps deployment to ASE 
* Azure DevOps Integration ? 
* Create a Key Vault (enabledForTemplateDeployment) to use to store secrets and certificates


# ARM over Terraform

* New Azure services and features are immediately available in ARM templates - it takes time for them to appear in Terraform on Ansible 
* Template deployments are handled through a single submission of the template, rather than through multiple imperative commands
* Template deployments undergo pre-flight validation.
* Template deployments are tracked in the Azure portal with deployment history being maintained.
