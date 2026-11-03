# Day 3 – Azure Virtual Machines, Storage and CLI

## Azure Virtual Machine
A virtual computer running on Azure infrastructure.

### VM Resources
- CPU: Processes instructions.
- RAM: Temporarily stores running data.
- Storage: Stores files and applications.

### VM Images
Preconfigured operating system images used to create VMs.

Example: Ubuntu Server.

## Azure Storage

- Blob Storage: Images, videos and files.
- File Storage: Shared folders.
- Queue Storage: Messages between application components.
- Table Storage: NoSQL structured data.

## Storage Redundancy

- LRS: Locally Redundant Storage.
- ZRS: Zone-Redundant Storage.
- GRS: Geo-Redundant Storage.

## Azure CLI

Azure CLI manages Azure resources through terminal commands.

### Commands Practised

az version
az login
az account show --output table
az account list --output table
az group list --output table
az vm list --output table

## VM Cost Management

- Running: VM is active.
- Stopped: Compute charges may continue.
- Deallocated: VM compute charges stop.

Note: Disks and other attached resources may still incur charges.