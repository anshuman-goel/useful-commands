# Useful Commands on Windows

#### Open File Explorer from Command Line
`start .`

#### Shortcut to open Windows Explorer
`Windows Key + E`

------
## Application Verifier
#### Enabling various tracking
`gflags -i <binary name> +hpa +ust +htc +hfc +htg`

#### Enabling Page Heap
`gflags /p /enable <binary name> /full`

#### Disable tracking
`gflags -i <binary name> -hpa -ust -htc -hfc -htg`

#### Disable Page Heap
`gflags /p /disable <binary name> /full`

---
## Azure Functions
#### Specifying Connection string in `local.settings.json`
```
{
  "IsEncrypted": false,
  "Values": {
    "AzureWebJobsStorage": "UseDevelopmentStorage=true;",
    "FUNCTIONS_WORKER_RUNTIME": "dotnet"
  },
  "ConnectionStrings": {
    "MyConnectionString": "[YourConnectionStringHere]"
  }
}
```
## Windbg
#### Ignore First Chance ASan Exceptions
`sxd av`
