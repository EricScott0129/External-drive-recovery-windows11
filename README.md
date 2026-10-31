# external-drive-recovery-windows11
# External Drive Recovery & Configuration – Windows 11

## Project Overview
Troubleshot, erased, partitioned, and reformatted a 500GB Maxone USB 3.0 external hard drive using Windows Disk Management and DiskPart.

## Initial Problem
The external drive was not appearing correctly in File Explorer. Windows recognized the device, but the storage was not accessible as expected.

## Tools & Technologies
- Windows 11
- Disk Management
- DiskPart
- NTFS File System
- GPT Partition Style
- USB 3.0 External Storage

## Troubleshooting Process
1. Identified the external drive using Disk Management.
2. Used `list disk` to identify the correct physical disk.
3. Verified the device using `detail disk`.
4. Used `clean` to remove existing partition information.
5. Converted the drive to GPT.
6. Created a new primary partition.
7. Formatted the partition using NTFS.
8. Assigned drive letter D:.
9. Verified the final storage capacity and file system.

## Troubleshooting Challenge
The initial NTFS formatting attempt returned a file-system compatibility error.

Inspected the partition layout, selected the primary partition, and successfully retried the NTFS quick format.

## Final Results
- Drive: Maxone USB 3.0
- Advertised Capacity: 500GB
- Usable Capacity: Approximately 465GB
- File System: NTFS
- Partition Style: GPT
- Drive Letter: D:
- Status: Healthy

## Storage Organization
Created folders for:
- Games
- Documents
- Pictures
- Videos
- IT Projects

## Skills Demonstrated
- Windows storage administration
- Command-line troubleshooting
- Disk partition management
- File-system configuration
- USB device troubleshooting
- Technical documentation

## Key Takeaway
Gained hands-on experience troubleshooting external storage, using Windows DiskPart commands, and restoring a drive to a usable state.
