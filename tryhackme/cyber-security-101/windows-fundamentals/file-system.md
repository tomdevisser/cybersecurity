# File system

## Systems

The file system in modern versions of Windows is the NTFS, _New Technology File System_. Before NFTS, there was FAT16/FAT32, _File Allocation Table_, and HPFS, _High Performance File System).

FAT partitions are still used today in e.g. USB devices, MicroSD cards.

NTFS is known as a journaling file system. In case of failure, it can automatically repair the folders/files on disk using information stored in a log file, which is not possible using FAT. It also addresses other limitations of previous file systems, such as:

- Files larger than 4GB
- Specific permissions on folders and files
- Folder and file compression
- Encryption (EFS, _Encryption File System_)

## Permissions

The possible permissons on NTFS volumes are:

- Full control
- Modify
- Read and execute
- List folder of contents
- Read
- Write

ADS, or _Alternate Data Streams_, is a file attribute specific to NTFS. Every file has at least one data stream ($DATA) and possibly more. Powershell gives you the ability to view ADS for files. Malware writers can utilise this to hide data. It can also have identifiers written to it to identify that a file was downloaded from the internet.

## Windows System folders

C:\Windows is known as the folder which contains the OS. It can reside in any other drive, and technically also in a different folder. The environment variable %windir% can tell you this.

One of the folders in Windows\ is System32. It holds the important files, critical for the operating system.

C:\Users will contain the profile folders for users. Each user will have some of the same folders, including Desktop, Documents and Downloads.
