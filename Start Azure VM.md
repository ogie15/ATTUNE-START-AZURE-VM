# This step starts the Azure Virtual Machine(s)

The script first gets the execution policy of the current PowerShell session.

Then checks if the execution policy is set to Unrestricted.

If it's not, it then sets the execution policy to Unrestricted for the current session.

Next, the AzPowerShell module is imported to the current session.

Then the values below are set:

1. UserName: This is the Username of the Azure Administrator corresponding to the `AzureUserName` set in the Inputs Tab.
1. PasswordString: This is the Password of the Azure Administrator corresponding to the `AzurePassword` set in the Inputs Tab.
1. AzureVmNames: This holds an array of VM(s) name(s) in Azure corresponding to the `AzureVmNames` set in the Inputs Tab.

Next, a connection to Azure is made.

Then it loops through the values of the Azure VM Names and starts the virtual machines.

Finally, the Azure PowerShell session is disconnected.
