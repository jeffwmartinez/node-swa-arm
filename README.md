# node-swa-arm

Command to deploy arm template with both azuredeploy.json and azuredeploy.parameters.json files

```cli
az deployment group create --resource-group my-rg --template-file azuredeploy.json --parameters azuredeploy.parameters.json --verbose
```