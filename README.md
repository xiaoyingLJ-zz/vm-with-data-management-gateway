# Create a virtual machine with gateway installed

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FxiaoyingLJ%2Fquick-create-vm-with-new-gateway%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FxiaoyingLJ%2Fquick-create-vm-with-new-gateway%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Prerequisites

- Name of existing data factory.
- Name of the Resource Group that the data factory resides in(This template must be in this resource group)
- Name of the existing VNET and subnet you want to connect the new virtual machine to.
- Name of the Resource Group that the VNET resides in.
- Region of the VNET(VM will be created in the same region with VNET)

```
NOTE

This template will create an additional storage account for vm system image and boot diagnostic.To avoid to running into storage account limits, it's best to delete the storage account when the VM is deleted
```

This template will create a gateway and help you make it workable in azure VM. The VM can join in an exsiting VNET.
