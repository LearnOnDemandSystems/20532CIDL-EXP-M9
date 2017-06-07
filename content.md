
<!---
Version: 1.0 
-->
# Exercise 1: Use xPlat CLI to Create and Manage and Azure Web App
## INTRODUCTION MESSAGE
In this exercise, you will:  
  
Install the Azure xPlat CLI package.  
Authenticate to Azure using the xPlat CLI.  
Create a Web App using the xPlat CLI.  
Remove the Web App using xPlat CLI  
  
The main tasks for this exercise are as follows:  
Install xPlat CLI.  
Authenticate to Azure by using xPlat CLI.  
Create a new Website instance by using xPlat CLI.  
Remove a Website instance by using xPlat CLI.
## COMPLETION MESSAGE
Results: After completing this exercise, you will have used xPlat CLI to manage instances of an Azure service.
### Login as Student
Login as Student with a password of Pa$$w0rd.

#### :bulb: KNOWLEDGE
You can use the Commands menu and choose Ctrl\+Alt\+Delete then click Student and enter Pa$$w0rd and press Enter. You can also use the Command menu and choose Paste/Paste Password instead of typing the password manually.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666817.jpg
>* ShowAutomatically = No





### On the Start screen, click Internet Explorer
On the Start screen, click the Internet Explorer tile

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666818.jpg
>* ShowAutomatically = No





### Go to the new Azure Portal
Go to https://portal.azure.com. Enter the email address of your Microsoft account associated with your Azure subscription. Then enter the password for your Microsoft account. Check Keep me signed in. Click Sign In.

#### :bulb: KNOWLEDGE
Before starting this lab, you must have completed the lab in Module 2. All work in this lab is done within vm20532 created in the lab in Module 2. Start and Connect via Azure Portal.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666819.jpg
>* ShowAutomatically = No



#### :calling: COMMAND
```TypeText
https://portal.azure.com
```


### Browse Virtual Machines
In the navigation pane on the left side of the Azure Portal, click Virtual Machines.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666820.jpg
>* ShowAutomatically = No





### Start the VM
Click the vm20532 VM that was created in the lab in Module 2 for development. In the Overview blade, if the VM is stopped, click Start and wait for the VM to start up. This may take a few minutes.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666821.jpg
>* ShowAutomatically = No





### Connect to the VM via RDP
When the vm20532 VM has started, click Connect.

#### :bulb: KNOWLEDGE
If prompted with a message "Internet Explorer blocked a pop-up from portal.azure.com", choose "Options for this site" and then select "Always Allow". Then try to Connect again.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666822.jpg
>* ShowAutomatically = No





### Allow pop-ups
If presented with a message box that shows a pop-up has been blocked, select Options for this site and choose Always Allow. Then click Connect again.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/672821.jpg





### Click Open
When presented with the RDP download pop-up at the bottom of the screen, click Open.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/672822.jpg





### In the Remote Desktop Connection dialog box:
In the Remote Desktop Connection dialog box, perform the following steps:  
a. Click Don’t ask me again for connections to this computer to prevent this dialog box from displaying again.  
b. Click Connect.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666823.jpg
>* ShowAutomatically = No





### In the Windows Security dialog box:
In the Windows Security dialog box, perform the following steps:  
a. For the User name dialog box, provide the value, Student.  
b. For the Password dialog box, provide the value, AzurePa$$w0rd.  
c. Click OK.

#### :bulb: KNOWLEDGE
Note: If you computer is on a domain, you may need to add a backslash before the username to "escape" the domain.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666824.jpg
>* ShowAutomatically = No





### In the Remote Desktop Connection dialog box:
In the Remote Desktop Connection dialog box, perform the following steps:  
a. Verify if the Remote certificate name matches the name of your virtual machine.  
b. Click Don’t ask me again for connections to this computer to prevent this dialog box from displaying again.  
c. Click Yes.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666825.jpg
>* ShowAutomatically = No





### Minimize Server Manager
If you just started the VM, Server Manager will start automatically after 30 seconds. If it starts, you can close it.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666826.jpg
>* ShowAutomatically = No





### Open the Microsoft Web Platform Installer app
Click the Start menu. Click the down-arrow to see all apps. Open the Microsoft Web Platform Installer application.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666827.jpg





### At Web Platform Installer dialog, click Products:
In the Web Platform Installer dialog, click the Products tab.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666828.jpg





### Locate Microsoft Azure Cross-platform Command Line
Click the Add button to the right of Microsoft Azure Cross-platform Command Line Tools option. Click the Install button.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666829.jpg





### Click the I Accept button.
You will be prompted with a list of pre-requisite applications. Click the I Accept button.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666830.jpg





### Wait for the installation process to complete:
Wait for the installation process to complete, then click Finish

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666831.jpg





### Open Command Prompt:
On the Start screen, type CMD, and then click Command Prompt. Switch to the Command Prompt window.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666832.jpg





### Validate that the azure CLI command is available:
To validate that the azure CLI command is available, type the following command in the console, and then press Enter:  
azure --help

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666833.jpg



#### :calling: COMMAND
```TypeText
azure --help
```


### Type Y to indicate you approve data collection:
Type Y and press Enter to indicate that you approve of the data collection process.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666834.jpg





### Switch to the ARM mode for the CLI:
To switch to the ARM mode for the CLI, type the following command in the console, and then press Enter:  
azure config mode arm

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666835.jpg



#### :calling: COMMAND
```TypeText
azure config mode arm
```


### Begin the interactive login process:
To begin the interactive login process, type the following command in the console, and then press Enter:  
azure login

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666836.jpg



#### :calling: COMMAND
```TypeText
azure login
```


### Note the code provided by the CLI:
Take a note of the code provided by the CLI command tool.

#### :bulb: KNOWLEDGE
Note: The code is displayed in the command prompt. For example, you may see: Enter the code FV7J9BJJL to authenticate. In this example, the code is FV7J9BJJL .





### On the Start screen, click Internet Explorer
On the Start screen, click the Internet Explorer tile. Go to https://aka.ms/devicelogin  
In the code dialog box, type in the code you recorded earlier. If the code is correct, the page will refresh automatically and render the name of the application requesting access to your Azure subscription \)Microsoft Azure CLI). Click the Continue button.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666838.jpg



#### :calling: COMMAND
```TypeText
https://aka.ms/devicelogin
```


### Sign In to your Azure subscription
In the email address dialog box, type the email address of your Microsoft account.  
In the password dialog box, type the password for your Microsoft account.  
Click Sign In.

#### :bulb: KNOWLEDGE
If prompted to use Auto Complete, choose No

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666839.jpg





### View Confirmation
View Confirmation page

#### :bulb: KNOWLEDGE
Note: If you were successful, you will see the message "You have signed in to the Microsoft Azure Cross-platform Command Line Interface application on your device". The code has a timeout so it is possible to not login quickly enough using the Device Login page. If this happens, simply repeat this task.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666840.jpg





### Return to Command Prompt, view account details:
Return to the Command Prompt application. To view your account details, type the following command in the console, and then press Enter:  
azure account show

#### :bulb: KNOWLEDGE
Note: If you have multiple Azure subscriptions, you can use azure account set \[subscription-name\] to select the appropriate subscription. If you are unsure about your subscription's name, you can simply use azure account list. If your Azure subscription is provided by a Learning Partner, it might be an auto-generated account without any details. In such a case, this command will return an empty result.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666841.jpg



#### :calling: COMMAND
```TypeText
azure account show
```



### View a list of your Resource Groups:
To view a list of your Resource Groups, type the following command in the console, and then press Enter: (You should see one pre-existing resource group listed - Make a note of it - you will need it later): 
azure group list

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666843.jpg



#### :calling: COMMAND
```TypeText
azure group list
```


### Create a new Web App Resource:
To create a new Web App Resource, type the following command in the console by providing the unique name selected for your Web App and your resource group name, then press Enter:  
azure resource create --name \[Unique Name\] --resource-type "Microsoft.Web/Sites" --api-version "2014-06-01" --location "East US" --resource-group \[Resource Group Name\]

#### :bulb: KNOWLEDGE
Note: You might get an error message notifying you that your Website’s name is not unique. If this occurs, select a new name until your Website is created.  
  
If you get a message "The subscription is not registered to use namespace 'Microsoft.Web'" you can try to issue the following command at the command line:  
azure provider register Microsoft.Web  
  
\)Note: if the command times out, try it again)  
  
If successful, try to create the Web App again.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666844.jpg



#### :calling: COMMAND
```TypeText
azure resource create --name [Unique Name] --resource-type "Microsoft.Web/Sites" --api-version "2014-06-01" --location "East US" --resource-group [Resource Group Name]
```


### View a list of Resources in the your resource group:
To view a list of Resources in your Resource Group, type the following command in the console, and then press Enter:  
azure resource list --resource-group \[Resource Group Name\]

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666845.jpg



#### :calling: COMMAND
```TypeText
azure resource list --resource-group [Resource Group Name]
```


### Get the details for your new Website:
To get the details for your new Website, type the following command in the console by providing the unique name selected for your Website and your resource group name, then press Enter:  
azure resource show --name \[Unique Name\] --resource-type "Microsoft.Web/Sites" --resource-group \[Resource Group Name\] --api-version "2014-06-01" --json

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666846.jpg



#### :calling: COMMAND
```TypeText
azure resource show --name [Unique Name] --resource-type "Microsoft.Web/Sites" --resource-group [Resource Group Name] --api-version "2014-06-01" --json
```


### Record the defaultHostName value:
Record the defaultHostName value from the list of key-value pairs that are generated by the previous command. Also record the sku value.  
           

#### :bulb: KNOWLEDGE
Note: this hostname property will look similar to this: "defaultHostName": "websitepiaxfa4veu6lw.azurewebsites.net".  
  
Note: this hostname property will look similar to this: "sku": "Free".

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666847.jpg





### View the new Website in Internet Explorer:
To view the new Website in Internet Explorer, type the following command in the console, replacing \[Host Name\} with your web app unique name, and then press Enter:  
explorer “http://\[Host Name\].azurewebsites.net”

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666848.jpg



#### :calling: COMMAND
```TypeText
explorer “http://[Host Name].azurewebsites.net”
```


### Verify that the new Website is running.
Verify that the new Website is running. Close Internet Explorer. Switch to the Command Prompt console window.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666849.jpg





### Remove your new Web App:
To remove your new Web App, type the following command in the console by providing the unique name selected for your Website and your resource group name, and then press Enter:   
azure resource delete --name \[Unique Name\] --resource-type "Microsoft.Web/Sites" --resource-group \[Resource Group Name\] --api-version "2014-06-01"  
Type Y to indicate that you want to remove the Web App, and then press Enter.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666850.jpg



#### :calling: COMMAND
```TypeText
azure resource delete --name [Unique Name] --resource-type "Microsoft.Web/Sites" --resource-group [Resource Group Name] --api-version "2014-06-01"
```


### Close all windows
Close all windows on the VM. Leave the RDP session running for the next exercise.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666853.jpg






# Exercise 2: Use PowerShell to Create and Manage a Resource Group
## INTRODUCTION MESSAGE
In this exercise, you will:  
  
Authenticate to Azure in Windows PowerShell by using Azure Active Directory.  
Switch the Azure modules in use by using Windows PowerShell.  
Create a resource group from a template by using Windows PowerShell.  
Delete a resource group by using Windows PowerShell.  
  
The main tasks for this exercise are as follows:  
Switch to the Azure Resource Manager PowerShell Modules.  
Create a resource group by using Windows PowerShell.  
Remove the resource group by using Windows PowerShell.
## COMPLETION MESSAGE
Results: After completing this exercise, you will have used Azure to interact with the Resource Manager, resource groups, and resource group templates.
### Start Windows PowerShell.
On the Start screen, click Windows PowerShell.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666854.jpg
>* ShowAutomatically = No





### Login to Azure Resource Manager mode:
Switch to the Windows PowerShell window. To switch modules, type the following command in the console, and then press Enter:  
Login-AzureRmAccount

#### :bulb: KNOWLEDGE
Note that you may have to wait a couple minutes for data collection to complete before proceeding.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666859.jpg



#### :calling: COMMAND
```TypeText
Login-AzureRmAccount
```


### Sign In to your Azure subscription
In the Sign in to your account dialog box, perform the following steps:  
a. Enter the email address of your Microsoft account.  
b. Enter the password for your Microsoft account.  
c. Click Sign In.

#### :bulb: KNOWLEDGE
If prompted to participate in data collection, ignore the message and let the cmdlet run for a few minutes until you are prompted to enter your Microsoft Account and password as normal.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666860.jpg





### View your current Azure PowerShell session context
To view your current Azure PowerShell session context type the following command in the console, and then press Enter:  
Get-AzureRmContext

#### :bulb: KNOWLEDGE
Note: If you have multiple Azure subscriptions, you can use Select-AzureRmSubscription to select the appropriate subscription.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666861.jpg



#### :calling: COMMAND
```TypeText
Get-AzureRmContext
```



### Provide the parameters for the template:
To provide the parameters for the template, type the following command in the console including your resource group name, press enter and then perform the following steps:  
New-AzureRmResourceGroupDeployment -ResourceGroupName \[Resource Group Name\] -TemplateFile "F:\\Mod09\\Labfiles\\azuredeploy.json"  
f. For the administratorLogin prompt, provide the value testuser, and then press Enter.  
g. For the administratorLoginPassword prompt, provide the value TestPa$$w0rd, and press Enter.

#### :bulb: KNOWLEDGE
Note: Wait for the provisioning process to complete. Status messages will be displayed periodically and the final message with the details will be displayed when provisioning is complete.  
  
Note: If you get an error "The subscription is not registered for the resource type 'components' in the location" then the issue is explained in this tech note:  
  
https://azure.microsoft.com/en-us/updates/application-insights-general-availability-in-additional-regions-and-resource-location-update-east-us-south-central-us-west-europe-and-north-europe/

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666863.jpg



#### :calling: COMMAND
```TypeText
New-AzureRmResourceGroupDeployment -ResourceGroupName [Resource Group Name] -TemplateFile "F:\Mod09\Labfiles\azuredeploy.json"
```


### Get the details of your resource group:
To get the details of your resource group, type the following command in the console by providing the unique name selected for your Website, and then press Enter:  
Get-AzureRmResourceGroup –ResourceGroupName \[Resource Group Name\]


#### :calling: COMMAND
```TypeText
Get-AzureRmResourceGroup –ResourceGroupName [Resource Group Name]
```


### Get the details of your new Web site
To get the details of your new Web site, type the following command in the console by providing the unique name selected for your Website and your resource group name, and then press Enter:  
\)Get-AzureRmResource -IsCollection -ResourceGroupName \[Resource Group Name\] -ResourceType "Microsoft.Web/sites" -ApiVersion 2015-08-01).Properties

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666865.jpg



#### :calling: COMMAND
```TypeText
(Get-AzureRmResource -IsCollection -ResourceGroupName [Resource Group Name] -ResourceType "Microsoft.Web/sites" -ApiVersion 2015-08-01).Properties
```


### Record the value of the hostNames property:
Record the value of the hostNames property from the JSON data generated by the previous command.  
           

#### :bulb: KNOWLEDGE
Note: this hostname property will look similar to this: DefaultHostName : websitepiaxfa4veu6lw.azurewebsites.net.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666866.jpg





### View the new Website in Internet Explorer
To view the new Website in Internet Explorer, type the following command in the console, replacing \[Host name\] with the web app unique name and then press Enter:  
explorer “http://\[Host Name\].azurewebsites.net”

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666867.jpg



#### :calling: COMMAND
```TypeText
explorer “http://[Host Name].azurewebsites.net”
```


### Verify that the new Website is running.
Verify that the new Website is running. Close Internet Explorer.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666868.jpg



### Close the Windows PowerShell console window
Close the Windows PowerShell console window

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666870.jpg





### Close RDP session
Close RDP session and click OK to disconnect





### Stop VM to save billing charges
If you are stopping labs for the day, on the vm2032 Overview page in the Azure Portal, click Stop to stop billing charges until you start labs again. If prompted, click Yes to stop the VM.

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666856.jpg
>* ShowAutomatically = No





### Close Internet Explorer
Close Internet Explorer to end the lab

#### :camera: SCREENSHOT
>LODSProperties
>* Uri = screens/666857.jpg
>* ShowAutomatically = No






