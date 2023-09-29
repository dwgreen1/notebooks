Microsoft Azure
================================

# Azure CLI
Create a resource group, same as existing resource group
```bash
LOCATION=$(az group show --name 'my-rg-group' --query location --out tsv)
RGNAME='my-new-rg'
az group create --name $RGNAME --location $LOCATION
az group show --name $RGNAME
```

List resource groups matching a name
```bash
group -list --query "[?starts_with(name, 'my-reg-prefix')].name --output tsv
```

Delete resoruce groups matching a name
```bash
az group list --query "[?starts_with(name,'az104-03')].[name]" --output tsv | 
xargs -L1 bash -c 'az group delete --name $0 --no-wait --yes'
```
