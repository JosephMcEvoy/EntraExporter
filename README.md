# Azure AD Exporter

The Azure AD Exporter is a PowerShell module that allows you to export your Azure AD / Identity related objects and settings.
You can run this as a nightly scheduled task or a DevOps component (Azure DevOps, GitHub, Jenkins) and commit the exported files to an internal GIT repository.
This way you can have a complete version history of your tenant settings.

##  Development Environment Setup
Use the following command to Test the Program on your development environment
```powershell
    Import-Module AzureADExporter.psd1
```

## Installing the module
```powershell
    Install-Module AzureADExporter
```

## Using the module

### Connecting to your tenant
```powershell
    Connect-AzureADExporter
```

### Exporting all objects and settings
```powershell
    Invoke-AADExporter -Path 'C:\AzureADBackup\'
```

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
