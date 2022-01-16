#### ARM
    - ARM provides Infrastructure as code.

### Azure Storage
- Azure provides different storage services. These are all under Azure Storage Accounts
    - Blob storage
        - Storage for the object, unstructed data such as text and binary.
    - Azure Queues
        - Provides storage for the messages.
        - A message could be <= 64kb
    - Azure Tables
        - For NoSQL data
        - Provides storage for key/value data and schema-less design
    - Azure Files
        - File share system
        - Could be mounted on multiple OSs - Windows, Linux and Mac
    - Azure Disks
        - Block level storage volumes
        - Provides storage capabilites for the VMs
        - Just like a physical disks - HDD, SDD disks
- Containers could be created in order to further categorize data into these above storage types
#### Azure Blob Storage 
    - Hierarchy of the blob - Storage Account >> Container  >> Blob
    - Containers withing blob storage are used to organize the blobs just like directories.
    - Types of blobs supported by AZ
        - Block blobs - contians blocks of data, text and binary data
        - Append blobs - same as block, optimized for append, good for logging output
        - Page blobs - random access files storage

#### Azure Files
    - Enables file share on the cloud.
    - Uses Server Message Block Protocol  (SMB) in order to do so.
    - Equivalent of the on-prem file server and could be mounted on the linux, windows and Mac server.

#### Azure Queues
    - Provides storage for the message which are used for communication among distributed application, these message could be up to 64kb in the size and AZ Queues are accesible through HTTP or HTTPS connections.

#### Azure Table Storage
    - Allows you store thge NoSQL database
    - A Table would contians several entities which need not share the same property and table does not enforce any schema on these entities.

#### Azure Managed Disks 
    - Azure Managed Disks are used for the VMs.
    - Disk Roles 
        - Data - Stores application data
        - OS - hosts the VM's OS and boot volume
        - TEMP - not a managed disk, store pages and swap files


#### Azure Blob Storage 
    - Page Blobs
	- Commonly used for virtual hard disks on Azure VM
	- Optimised for read and write - 512 byte
    - Block Blobs
	- Storage large blobs (4.75TB)
	- Blobs could be deleted or updated
    - Append Blobs
	- Optimised for append operation
	- Inseration at the end of the blob only
	- Can not be deleted or updated
    - Moving blobs between Storage Containers	
	- It is not supported natively.
	- It could be achieved with AzCopy tool.
	- Data Movement Library can also help in such operation.
    - Moving blobs between Storage Accounts
	- AzCopy is helpful here.
    - Blob leasing provides ownership of the blob for given time period or indefinitely and it makes sure that blob is read-only during lease period
    - Tiers in decreasing order of the cost - Premium - Hot - Cold - Archive
    - Retention Policies - Time Based & Legal Hold