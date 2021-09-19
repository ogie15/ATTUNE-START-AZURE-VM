# This step starts the Azure Virtual Machine(s)

- *The script first gets the execution policy of the current PowerShell session.*
- *Then checks if the execution policy is set  to Unrestricted.*
- *If it's not, it then sets the execution policy to Unrestricted for the current session.*

---

First, the AzPowerShell module is imported to the current session.

Then the values below are set:

1. UserName: This is the Username of the Azure Administrator (DataType: String)
1. PasswordString: This is the Password of the Azure Administrator (DataType: String)
1. AzureVmNames: This holds an array of VM(s) name(s) in Azure (DataType: Array)

---

The Array holds the value of the Azure Virtual Machine names.

*Array Syntax:*

```powershell
@('VMOne', 'VMTwo', 'VMThree')
```

---

**NOTE**: *The `Azure Virtual Machine Names` are gotten from the Array created in Attune.*
