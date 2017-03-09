## UCS Director Exchange 2012 Rollout

UCS Director by itself offers many ways to integrate different solutions. For example, there is always the option to create granular individual Workflows by integrating existing scripts. In addition, you could also use "Open Automation" or "Script Modules".


### Prerequisites

Before we begin to create the workflow, we need to have a working Windows 2012 image and a running PowerShell Agent which is integrated into UCS Director. Ideally, the install files are available for Exchange.

### Starting with the workflow
Notice: All the required information are in the attached workflow at the end of the post as well. If you want to skip, please feel free :-)

![Catalog Item Exchange 2012](https://github.com/sthellwi/UCS-Director/blob/master/images/exchange01.png?raw=true)

Based on the screenshot we are starting with generic VM settings. Afterwards we are going into the PowerShell configuration and create the dependencies for the Exchange Server 2012.



```markdown
# Install Microsoft Exchange 2012 dependencies
echo "Install-WindowsFeature Net-HTTP-Activation, Desktop-Experience, NET-Framework-45-Features, RPC-over-HTTP-prox y, RSAT-Clustering, RSAT-Clustering-CmdInterface, RSAT-Clustering-Mgmt, RSAT-Clustering-PowerShell, Web-Mgmt-Console, WAS-Process-Model, Web-Asp-Net45, Web-Basic-Auth, Web-Client-Auth, Web-Digest-Auth, Web-Dir-Browsing, Web-Dyn-Compress ion, Web-Http-Errors, Web-Http-Logging, Web-Http-Redirect, Web-Http-Tracing, Web-ISAPI-Ext, Web-ISAPI-Filter, Web-Lgcy -Mgmt-Console, Web-Metabase, Web-Mgmt-Console, Web-Mgmt-Service, Web-Net-Ext45, Web-Request-Monitor, Web-Server, Web-S tat-Compression, Web-Static-Content, Web-Windows-Auth, Web-WMI, Windows-Identity-Foundation, RSAT-ADDS" >c:\\ex-depen. ps1
c:\\ex-depen.ps1
```


### Support or Contact
Any questions about the workflow?
My e-mail is [sthellwi@cisco.com](mailto:sthellwi@cisco.com).
