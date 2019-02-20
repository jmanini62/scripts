# Download the Cohesity SQL PowerShell Scripts

There are three SQL related scripts that are often useful to SQL DBAs. They are:

* restore-SQL.ps1: restore a SQL database for operational recovery or testing. View the readme for this script at https://github.com/bseltz-cohesity/scripts/tree/master/powershell/SQLrestore

* sqlClone.ps1: clone a SQL database for test/dev. View the readme for this script at https://github.com/bseltz-cohesity/scripts/tree/master/powershell/SQLClone

* destroyClone.ps1: tear down a SQL clone. View the readme for thids script at https://github.com/bseltz-cohesity/scripts/tree/master/powershell/destroyClone

You can download these scripts onto your PC by opening a PowerShell session and running the following commands:

```powershell
md cohesity-sql-scripts
cd cohesity-sql-scripts
Invoke-WebRequest -Uri https://raw.githubusercontent.com/bseltz-cohesity/scripts/master/powershell/SQLrestore/cohesity-api.ps1 -OutFile cohesity-api.ps1
Invoke-WebRequest -Uri https://raw.githubusercontent.com/bseltz-cohesity/scripts/master/powershell/SQLrestore/restore-SQL.ps1 -OutFile restore-SQL.ps1
Invoke-WebRequest -Uri https://raw.githubusercontent.com/bseltz-cohesity/scripts/master/powershell/SQLClone/sqlClone.ps1 -OutFile sqlClone.ps1
Invoke-WebRequest -Uri https://raw.githubusercontent.com/bseltz-cohesity/scripts/master/powershell/destroyClone/destroyClone.ps1 -OutFile destroyClone.ps1
```