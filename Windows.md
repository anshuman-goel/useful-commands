# Useful Commands on Windows

#### Open File Explorer from Command Line
`start .`

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
