## Getting Started:


###### Description

The Action Pack can be used for running commands on remote Windows machines.
The "Run Commands" Action takes a script block as input and runs it on a target machine. You can type Powershell or batch commands in different lines in the web interface of your CA Automic One Automation Platform. You can specify file names on the agent machine where the standard output and the standard error will be written. The Job Log will contain the standard output and the standard error of the commands. A variable captures the error code of the last executed command. You can specify a return code to capture in order to consider the Action ends in a success status.
		
###### Actions

1. Run Commands
		
###### Compatibility:

1. Microsoft .Net 4
2. Open JDK Java 11 
3. Oracle Java 1.7 

###### Prerequisite:

1. ITPA Shared and FileSystem action packs should be installed.
2. A Windows automation agent (it will be the WinRM client)
3. The Agent machine and the remote machines (WinRM servers) must be in the same network domain
4. WinRM must be enabled on both the agent machine and the remote machines
5. A network connection from the agent machine to the target machines
	1. Default HTTP port: 5985
	2. Default HTTPS port: 5986
After you have installed the Action Pack in your CA Automic One Automation Platform, you will find a documentation object with full documentation.

###### Steps to install action pack source code:

1. Clone the code to your machine.
2. Go to the package directory.
3. Run the command apm upload in the directory which contains package.yml (source/):
   Ex. **apm upload -force -u <Name>/<Department> -c <Client-id> -H <Host> -pw <Password> -S AUTOMIC -y -ia -ru**


###### Package/Action Documentation

Please refer to the link for [package documentation](source/ae/DOCUMENTATION/PCK.AUTOMIC_MICROSOFT_WINRM.PUB.DOC.xml)

###### Third party licenses:

The third-party library and license document reference.[Third party licenses](source/ae/DOCUMENTATION/PCK.AUTOMIC_MICROSOFT_WINRM.PUB.LICENSES.xml)

###### Useful References

1. [About Packs and Plug-ins](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#PluginManager/PM_AboutPacksandPlugins.htm?Highlight=Action%20packs)
2. [Working with Packs and Plug-ins](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#PluginManager/PM_WorkingWith.htm#link10)
3. [Actions and Action Packs](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#_Common/ReleaseHighlights/RH_Plugin_PackageManager.htm?Highlight=Action%20packs)
4. [PACKS Compatibility Mode](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#AWA/Variables/UC_CLIENT_SETTINGS/UC_CLIENT_PACKS_COMPATIBILITY_MODE.htm?Highlight=Action%20packs)
5. [Working with actions](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#ActionBuilder/AB_WorkingWith.htm#link4)
6. [Installing and Configuring the Action Builder](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#ActionBuilder/install_configure_plugins_AB.htm?Highlight=Action%20packs)

###### Distribution: 

In the distribution process, we can download the existing or updated action package from the Automation Engine by using the apm build command.
Example: **apm build -y -H AE_HOST -c 106 -u TEST/TEST -pw password -d /directory/ -o zip -v action_pack_name**
			
			
###### Copyright and License: 

Broadcom does not support, maintain or warrant Solutions, Templates, Actions and any other content published on the Community and is subject to Broadcom Community [Terms and Conditions](https://community.broadcom.com/termsandconditions)

###### Questions or Need Help? 

Join the [Automic Community Integrations](https://community.broadcom.com/communities/community-home?CommunityKey=83e49dd4-b93e-464a-a343-2bb1e51c13ec) to discuss this integration.
