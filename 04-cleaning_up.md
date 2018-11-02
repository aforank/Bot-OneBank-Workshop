# Cleaning Up

In this lab, you will remove the resource group containing your Service Fabric resources and Bot Channel resources.

## Removing Lab Assets

*In many Azure scenarios, your entire application solution is grouped into an Azure resource group. You will use the Cloud Shell tool in the Azure Portal to list all of your resource groups and then delete the resource group you used for these labs.*

### Open Cloud Shell

1. At the top of the portal, click the **Cloud Shell** icon to open a new shell instance.

    > If this is your first time using the cloud shell, you may need to configure the default Storage account and SMB file share.

### Use Azure CLI to Delete Resource Group

1. In the **Cloud Shell** command prompt at the bottom of the portal, type in the following command and press **Enter** to list all resource groups in the subscription:

    ```sh
    az group list
    ```

1. Type in the following command and press **Enter** to delete the **ONEBANKRG** *Resource Group*:

    ```sh
    az group delete --name ONEBANKRG --no-wait --yes
    ```

1. Close the **Cloud Shell** prompt at the bottom of the portal.

1. Close your browser application.
