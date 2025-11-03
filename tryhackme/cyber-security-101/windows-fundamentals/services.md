# Services

## Windows Update

Windows Update is a service provided by Microsoft to provide security updates, feature enhancements, and patches for the Windows operating system and other Microsoft products, such as Microsoft Defender.

Updates are typically released on the 2nd Tuesday of each month. This day is called Patch Tuesday. That doesn't necessarily mean that a critical update/patch has to wait for the next Patch Tuesday to be released. If the update is urgent, then Microsoft will push the update via the Windows Update service to the Windows devices.

## Windows Security

Windows Security has several _Protection areas_:

- Virus & threat protection
- Firewall & network protection
- App & browser control
- Device security

### Virus & threat protection

There are two parts: current threats, and virus and threat protection settings.

Current threats can perform a quick, full or custom scan. Quick scan checks only the folders where threats are often found, and custom lets you decide which folders to check. Threat history contains the last scan, quarantined threats and allowed threats.

Virus and threat protection settings lets you check for updates, and manage settings.

- Real-time protection
- Cloud-delivered protection
- Automatic sample submission
- Controlled folder access
- Exclusions
- Notifications

You can also enable ransomware protection by enabling real-time protection and controlled folder access.

### Firewall & network protection

Windows Firewall offers three firewall profiles: domain, private and public.

Domain - The domain profile applies to networks where the host system can authenticate to a domain controller. 
Private - The private profile is a user-assigned profile and is used to designate private or home networks.
Public - The default profile is the public profile, used to designate public networks such as Wi-Fi hotspots at coffee shops, airports, and other locations.

### App & browser control

Microsoft Defender SmartScreen protects against phishing or malware websites and applications, and the downloading of potentially malicious files.

### Device security

Built-in security. Includes core isolation, which is virtualisation-based security. And a security processor, called TPM (_trusted platform module_), providing additional encryption.

Trusted Platform Module (TPM) technology is designed to provide hardware-based, security-related functions. A TPM chip is a secure crypto-processor that is designed to carry out cryptographic operations. The chip includes multiple physical security mechanisms to make it tamper-resistant, and malicious software is unable to tamper with the security functions of the TPM.

## BitLocker

BitLocker Drive Encryption is a data protection feature that integrates with the operating system and addresses the threats of data theft or exposure from lost, stolen, or inappropriately decommissioned computers. BitLocker provides the most protection when used with a Trusted Platform Module (TPM) version 1.2 or later. The TPM is a hardware component installed in many newer computers by the computer manufacturers. It works with BitLocker to help protect user data and to ensure that a computer has not been tampered with while the system was offline.

## Volume Shadow Copy Service

The Volume Shadow Copy Service (VSS) coordinates the required actions to create a consistent shadow copy (also known as a snapshot or a point-in-time copy) of the data that is to be backed up. Volume Shadow Copies are stored on the System Volume Information folder on each drive that has protection enabled.

If VSS is enabled (System Protection turned on), you can perform the following tasks from within advanced system settings. 

- Create a restore point
- Perform system restore
- Configure restore settings
- Delete restore points

From a security perspective, malware writers know of this Windows feature and write code in their malware to look for these files and delete them. Doing so makes it impossible to recover from a ransomware attack unless you have an offline/off-site backup.
