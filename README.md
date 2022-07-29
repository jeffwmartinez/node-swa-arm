# node-swa-arm

Command to deploy arm template with both azuredeploycosmos.json and azuredeploycosmos.parameters.json files

```cli
az deployment group create --resource-group my-rg --template-file azuredeploycosmos.json --parameters azuredeploycosmos.parameters.json --verbose
```
This will deploy an arm template that creates the following resources
1. Static Web App
2. Cosmos DB w/ Mongo DB API

NOTES:
1. In the `azuredeploycosmos.parameters.json` file: replace the `repositoryUrl` and `repositoryToken` values with your github repo url and a github Personal Access Token
2. Once deployed, grab the PRIMARY KEY value from your Cosmos DB resource and paste it in the COSMOS_CONNECTION_STRING app setting value
